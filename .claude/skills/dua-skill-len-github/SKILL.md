---
name: dua-skill-len-github
description: Đưa một skill (skill có sẵn trong tài khoản, nội dung SKILL.md người dùng dán vào, hoặc skill mới cần viết) vào code tại .claude/skills/<tên>/, viết README tiếng Việt, commit và đẩy lên repo GitHub của người dùng, kiểm tra kết quả trên GitHub và hướng dẫn cách thấy/dùng skill trong Claude. Dùng khi người dùng nói "đưa skill vào code", "lưu skill lên GitHub", "đẩy skill lên repo", "/dua-skill-len-github".
---

# Đưa skill vào code và lưu lên GitHub

Làm việc bằng **tiếng Việt**, câu ngắn, dễ hiểu. Người dùng thường không rành kỹ thuật: tự làm mọi việc làm được, chỉ nhờ người dùng những bước bắt buộc phải tự làm (tạo repo, cấp quyền GitHub).

## Bước 1. Xác định skill cần đưa vào

Theo thứ tự ưu tiên:
1. Người dùng nêu tên skill → tìm trong `~/.claude/skills/` (kể cả `~/.claude/skills/synced/*/`) và `~/.claude/plugins/`.
2. Người dùng dán nội dung SKILL.md → dùng nguyên nội dung đó.
3. Người dùng mô tả một skill mới → viết SKILL.md mới (có frontmatter `name`, `description`).
4. Không nói rõ → liệt kê skill riêng của người dùng (bỏ qua skill chuẩn của Anthropic như docx, pdf, pptx, xlsx, skill-creator, import-memory, google-workspace, morning, docs). Nếu chỉ có một skill riêng thì chọn luôn; nếu nhiều thì hỏi một câu.

Đọc toàn bộ skill trước khi chép. Chép **cả thư mục** skill (gồm scripts, references, assets nếu có), không chỉ SKILL.md.

## Bước 2. Đặt skill vào code

```
<repo>/
├── README.md
└── .claude/skills/<tên-skill>/SKILL.md
```

- Nếu repo đã có sẵn trong phiên: thêm vào repo đó, không ghi đè skill trùng tên khi chưa hỏi.
- README.md viết tiếng Việt: skill làm gì, nằm ở đâu, cách gọi (`/<tên-skill>` hoặc nói tự nhiên). Nếu đã có README thì thêm mục mới, không xoá nội dung cũ.
- Commit với email người dùng, message tiếng Việt, ví dụ: `Thêm skill <tên-skill> vào project`.

## Bước 3. Đẩy lên GitHub

Những điều đã biết (đừng thử lại vô ích):
- **Không tạo được repo mới** từ phiên cloud (API `user/repos` bị chặn). Người dùng phải tự tạo repo trống tại https://github.com/new (không tick tạo README) rồi gửi link.
- Có link repo → gọi `add_repo` với `access: "push"`, clone về `/home/user/<repo>` (timeout dài), rồi gọi `register_repo_root`.
- Repo trống: `git fetch <thư-mục-có-commit> main && git checkout -B main FETCH_HEAD`, sau đó `git push -u origin main`.
- Push bị **403 "Claude doesn't have GitHub access"** → nhờ người dùng cài Claude GitHub App: https://github.com/apps/claude/installations/select_target, chọn đúng tài khoản và repo, bấm Install. Nếu vẫn lỗi: kết nối lại tại https://claude.ai/customize/connectors?auth_start=github&auth_start_force=1. Xong thì push lại.
- Cảnh báo `push negotiation failed; proceeding anyway` là **vô hại** nếu dòng cuối có `[new branch] main -> main` hoặc `main -> main`.
- Trong lúc chờ người dùng, gói code thành zip (`git archive --format=zip`) và gửi file để không mất code khi phiên kết thúc.

## Bước 4. Kiểm tra trên GitHub

Không tự nhận "thành công" trước khi kiểm tra:
```bash
git ls-remote origin
gh api "repos/<owner>/<repo>/git/trees/main?recursive=1" --jq '.tree[] | "\(.type) \(.path) \(.size // "")"'
```
Mã commit trên GitHub phải trùng commit trong phiên, và đủ các file đã thêm.

## Bước 5. Báo kết quả cho người dùng

Câu đầu tiên là kết quả (thành công hay chưa) kèm link repo. Sau đó:
- Cây thư mục đã lên GitHub.
- Nói rõ repo chỉ chứa gì (ví dụ: chỉ có skill + README, chưa có code website).
- Cách thấy và dùng skill:
  - **Claude Code** (claude.ai/code): tạo phiên mới → bấm nút **Repo** dưới ô chat → chọn repo → gửi một câu để bắt đầu → gõ `/` sẽ thấy `/<tên-skill>`.
  - Màn hình "Phiên mới" **không** hiển thị danh sách skill; đây là thiết kế của giao diện, không phải lỗi.
  - Xem skill của tài khoản: cột trái → **Tùy chỉnh** → **Skills**.
  - Chat thường của Claude không đọc skill từ repo GitHub; nó dùng skill trong tài khoản.
- Nếu người dùng muốn, có thể tạo sẵn một phiên Claude Code gắn repo bằng `create_session` (với `source_url` là link repo) để họ chỉ cần bấm vào trong mục **Gần đây**.
