# Mẫu landing page ưu đãi – Đồ ăn giao tận nơi

## Trong thư mục này có gì

| File | Dùng để |
|---|---|
| `landing-blogger.html` | Nội dung **dán vào Blogger** (Trang → Trang mới → chế độ HTML). |
| `xem-truoc.html` | Mở bằng trình duyệt để **xem thử** trên máy. Không dán file này vào Blogger. |

Trang có 5 nút đăng ký. Bấm nút nào cũng mở form 4 bước: **Đăng ký → Đặt cọc qua QR → Gửi ảnh qua Zalo → Xong (chia sẻ cho 5 bạn)**.

Form khách điền gồm: số điện thoại/Zalo, họ tên, địa chỉ giao, khung giờ nhận (trưa/chiều/tối), số phần ăn, món quan tâm (không bắt buộc), ghi chú/email (không bắt buộc).

## Bước 1 – Điền thông tin quán (chỉ sửa khối `CFG` ở đầu file)

Mở `landing-blogger.html`, điền vào giữa hai dấu `""`:

| Ô | Điền gì | Ví dụ |
|---|---|---|
| `ten` | Tên quán | Bếp Nhà Mây |
| `slogan` | Câu giới thiệu ngắn | Cơm nhà nấu mỗi ngày, giao tận nơi |
| `hotline`, `zalo` | Số điện thoại, số Zalo (Zalo để trống = dùng hotline) | 0912345678 |
| `diaChi`, `gioMoCua`, `khuVucGiao` | Địa chỉ bếp, giờ mở cửa, khu vực giao | |
| `tenUuDai`, `moTaUuDai` | Tên và mô tả ưu đãi | Combo 2 người 199K / Tặng 2 trà đào… |
| `giaGoc`, `giaUuDai`, `soSuat` | Giá gạch ngang, giá ưu đãi, số suất | 289.000đ / 199.000đ / 30 |
| `coc` | Tiền cọc, **chỉ ghi số** | 50000 |
| `bankId` | Mã BIN ngân hàng | Vietcombank 970436 · Techcombank 970407 · MB 970422 · ACB 970416 · BIDV 970418 · VietinBank 970415 · Agribank 970405 · VPBank 970432 · TPBank 970423 · Sacombank 970403 |
| `bankName`, `soTaiKhoan`, `chuTaiKhoan` | Ngân hàng, STK, tên chủ TK (viết HOA không dấu) | |
| `maCK` | Mã nội dung chuyển khoản, ngắn, không dấu | MAY199 |
| `maps`, `fanpage`, `tiktok` | Đường link | |
| `posterUrl` | Link ảnh poster đã tải lên Blogger (đổi kích thước thành `/s1600/`) | |

Ô nào chưa điền sẽ hiện chữ vàng **[CHƯA ĐIỀN …]** để dễ thấy.

Phần **thực đơn nổi bật**, **đánh giá khách hàng** và **vì sao chọn chúng tôi** đang để chữ trong ngoặc vuông `[...]`. Bạn thay bằng món, ảnh và lời giới thiệu thật của quán. Chỉ dùng đánh giá của khách thật đã đồng ý cho đăng. Nếu chưa có đánh giá nào thì xoá cả khối.

Nội dung chuyển khoản sẽ tự thành: `MÃCK MÃĐỐITÁC SĐTKHÁCH`, ví dụ `MAY199 MAI 0912345678`.

## Bước 2 – Google Form để theo dõi (khi muốn đếm số liệu và hoa hồng đối tác)

Tạo Form ở `forms.new`. Tất cả câu hỏi là **Trả lời ngắn**, không bắt buộc, đặt tên **đúng thứ tự** sau:

`loai, aff, vid, info, ten, sdt, email, diachi, khunggio, sophan, sangloc, nentang, thietbi`

Sau khi liên kết Form với Google Sheets, tab dữ liệu (đổi tên thành **DuLieu**) sẽ có các cột:

A Dấu thời gian · B loai · C aff · D vid · E info · F ten · G sdt · H email · I diachi · J khunggio · K sophan · L sangloc · **M nentang** · **N thietbi** · **O trangthai** (cột bạn tự thêm, gõ "Đã cọc").

Lấy mã Form và mã từng câu hỏi (entry), rồi điền vào `formId` và `entry` trong `CFG`. Mình sẽ làm giúp bạn bước này. Khi chưa điền, trang vẫn chạy bình thường, chỉ chưa ghi số liệu.

## Lưu ý quan trọng

- Trang web **không tự kiểm tra được tiền đã về tài khoản**. Vì vậy khách phải gửi ảnh chuyển khoản qua Zalo, và quán tự đối chiếu. Nếu muốn tự động hoá, có thể tìm hiểu SePay hoặc Casso (có tính phí).
- Lượt "chia sẻ" chỉ đếm số lần khách bấm nút chia sẻ, không biết bạn bè có nhận được hay không.
- Mã QR do vietqr.io tạo. Sau khi đưa trang lên Blogger, hãy quét thử bằng app ngân hàng để kiểm tra đúng tài khoản, số tiền và nội dung.

## Các bước tiếp theo

1. Điền khối `CFG` (hoặc gửi thông tin để mình điền giúp).
2. Mua tên miền (**bạn tự thanh toán**, nhớ xác thực email và eKYC trong 15 ngày).
3. Tạo blog trên Blogger, gắn tên miền, cài theme website.
4. Tạo trang landing, dán `landing-blogger.html`.
5. Tạo Google Form và Google Sheets (tabs DoiTac, TongHop, NenTang, DuLieu).
6. Thêm đoạn mã sửa link affiliate gõ sai và Microsoft Clarity vào theme.
7. Chạy thử với dữ liệu "TEST xoa", **xoá dữ liệu thử**, rồi bàn giao.
