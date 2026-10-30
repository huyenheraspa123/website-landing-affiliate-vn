---
name: "website-landing-affiliate-vn"
description: Dựng website Blogger + tên miền, landing page ưu đãi có form đăng ký 4 bước, đặt cọc VietQR, theo dõi affiliate/nền tảng bằng Google Form-Sheets và heatmap Clarity cho doanh nghiệp Việt.
---

# Website + Landing page ưu đãi + Affiliate (Quy trình chuẩn A–Z)

Quy trình này dựng cho **một doanh nghiệp nhỏ bất kỳ** (spa, nha khoa, phòng gym, quán ăn, trung tâm tiếng Anh, bất động sản, shop online…):

1. Website chuyên nghiệp **miễn phí** trên Blogger, gắn tên miền riêng, khách tự đăng bài được.
2. **Landing page chiến dịch ưu đãi**, gồm: poster, 5 nút đăng ký, form 4 bước (Đăng ký → Chuyển khoản QR → Gửi ảnh Zalo → Thành công + chia sẻ 5 bạn).
3. **Đặt cọc bằng VietQR**: số tiền và nội dung tự điền, có kèm mã đối tác và SĐT khách.
4. **Theo dõi affiliate miễn phí** bằng Google Form và Google Sheets. Thống kê truy cập, đăng ký, tỷ lệ, hoa hồng, nền tảng (Facebook/Zalo/TikTok…) và thiết bị (điện thoại/máy tính).
5. **Heatmap** bằng Microsoft Clarity.

Làm việc bằng **tiếng Việt** với khách, xưng hô theo cách khách dùng.

---

## 0. Nguyên tắc an toàn (BẮT BUỘC)

- **Khách tự làm** các việc sau, agent không làm thay: mua tên miền và thanh toán, đăng nhập, tạo tài khoản, xác minh danh tính (eKYC), bấm "Cho phép" ở cửa sổ OAuth của Google.
- **Phải hỏi và chờ khách đồng ý rõ ràng** trước khi: chấp nhận điều khoản (Terms), xuất bản hoặc đăng công khai, gửi tin thay khách, nhập dữ liệu cá nhân vào form.
- **Không bịa** đánh giá, lời chứng thực hay số liệu. Ảnh khách hàng chỉ dùng khi chủ doanh nghiệp xác nhận đã xin phép.
- **Dữ liệu thử** phải đặt tên dễ nhận biết (ví dụ "TEST xoa", SĐT 0900000000) và **xoá ngay sau khi test**. Không bao giờ xoá dữ liệu thật của khách.
- **Nói rõ giới hạn:** trang web tĩnh **không tự xác minh được tiền đã về tài khoản**. Thay bằng bước "gửi ảnh chuyển khoản qua Zalo". Nếu khách muốn tự động hoá bước này, gợi ý dịch vụ đọc biến động số dư (ví dụ SePay, Casso) và nói rõ cần tìm hiểu chi phí.
- Thông tin pháp lý, tài chính: chỉ cung cấp dữ kiện, không khuyên đầu tư.

---

## 1. Thu thập thông tin (hỏi 1 lần, đủ rồi mới làm)

Dùng AskUserQuestion hoặc hỏi gọn. Biến cần có:

| Biến | Ví dụ |
|---|---|
| THUONG_HIEU | Huyền Hera Beauty & Spa |
| LINH_VUC, DIA_CHI, GIO_MO_CUA | Spa · Số 17 Xuân Hòa, Thái Nguyên · 8:00–20:30 |
| HOTLINE / ZALO_SO | 0867312977 |
| DICH_VU (danh sách), KINH_NGHIEM | chăm sóc da, triệt lông… · 10 năm |
| LINK_MAPS, FANPAGE, FACEBOOK, TIKTOK | link thật của khách |
| TEN_MIEN mong muốn | tenthuonghieu.com |
| TEN_UU_DAI, MO_TA_UU_DAI_NGAN | "ưu đãi chăm sóc da 99K", "tặng thải độc da trị giá 250K (còn 0đ), 20 suất" |
| TIEN_COC_SO / TIEN_COC_HIEN_THI | 99000 / 99.000đ |
| BIN_NGAN_HANG, SO_TAI_KHOAN, CHU_TAI_KHOAN | 970407 (Techcombank), … |
| MA_NOI_DUNG_CK | HERA99 (ngắn, không dấu) |
| CAU_HOI_SANG_LOC + các lựa chọn | Spa: "Tình trạng da". Nha khoa: "Vấn đề răng". Gym: "Mục tiêu tập". Tiếng Anh: "Trình độ hiện tại" |
| Danh sách ĐỐI TÁC (mã, tên, % hoặc tiền hoa hồng) | MAI – 30.000đ/khách đã cọc |
| Ảnh: logo, poster ưu đãi, ảnh chủ, ảnh review (đã xin phép) | |

**BIN ngân hàng VietQR thường gặp:** Vietcombank 970436 · Techcombank 970407 · MB 970422 · ACB 970416 · BIDV 970418 · VietinBank 970415 · Agribank 970405 · VPBank 970432 · TPBank 970423 · Sacombank 970403. Nếu không chắc, kiểm tra lại trên vietqr.io.

Sau khi có đủ, tạo task list cho các bước 2–9, và thêm một bước kiểm tra cuối.

---

## 2. Tên miền

1. Mở trang mua tên miền (Mắt Bão, PA Việt Nam, Nhân Hòa, Namecheap…). **Khách tự bấm thanh toán.**
2. Nhắc khách: xác nhận email chủ thể trong 15 ngày và hoàn tất eKYC (tên miền .vn hoặc nhà đăng ký VN), nếu không tên miền có thể bị khoá.
3. Cấu hình DNS sau bước 3 (Blogger sẽ đưa 2 bản ghi CNAME):
   - `www` → CNAME → `ghs.google.com`
   - Bản ghi xác minh do Blogger cung cấp (CNAME tên dài → `gv-xxxx.dv.googlehosted.com`)
   - Tên miền gốc (@): A → `216.239.32.21`, `216.239.34.21`, `216.239.36.21`, `216.239.38.21`, rồi bật "Chuyển hướng tên miền gốc sang www" trong Blogger.
   - Tên miền phụ cho chiến dịch (ví dụ `uudai.tenmien.com`): dùng REDIRECT/URL forward của nhà đăng ký, trỏ về trang landing.

---

## 3. Website Blogger

1. Khách tự đăng nhập Google, vào blogger.com và tạo blog (khách bấm tạo).
2. **Chủ đề → Chỉnh sửa HTML:** dán theme tuỳ biến.
   - **Phải giữ lại** toàn bộ widget bị khoá (`locked='true'`) của theme Contempo gốc. Đặt chúng trong `<div class='hh-hidden' style='display:none'>` thay vì xoá. Giữ `b:defaultmarkups`. Đặt `Blog1` trong `page_body`. Nếu cần form liên hệ thì dùng widget `ContactForm`. Xoá widget khoá sẽ làm Blogger báo lỗi hoặc hiện "no-items".
   - Theme cần có: header + menu, trang chủ (giới thiệu, dịch vụ, quy trình, bảng giá, đánh giá, bản đồ, CTA), footer (hotline nút sao chép, email, địa chỉ, giờ mở cửa, mạng xã hội), nút gọi nổi.
   - Nếu theme chứa `&` hoặc `<` trong `<script>`, bọc nội dung script bằng `//<![CDATA[ … //]]>`.
3. **Cài đặt → Xuất bản → Tên miền tuỳ chỉnh:** nhập `www.tenmien.com`. Blogger hiện bản ghi xác minh, thêm vào DNS (bước 2), đợi rồi bật HTTPS.
4. Tạo các **Trang tĩnh** (Giới thiệu, Bảng giá, Liên hệ) và nhãn bài viết (Kiến thức).
5. Hướng dẫn khách tự đăng bài: Bài đăng mới → tiêu đề → ảnh hoặc video → nhãn → Xuất bản.

**Mẹo sửa nội dung bằng trình duyệt (agent):**

- Trình soạn HTML là CodeMirror: `document.querySelector('.CodeMirror').CodeMirror.getValue()` và `.setValue(v)`.
- Sau `setValue`, Blogger chưa nhận là có thay đổi. Phải click vào editor, bấm `Ctrl+End`, gõ 1 dấu cách, Backspace, rồi mới bấm **Cập nhật** (trang) hoặc **Lưu** (theme).
- Khi `replace` chuỗi có ký tự `$` (ví dụ `'$1 $2'`), luôn dùng hàm: `v.replace(old, () => newStr)`.
- Sửa bằng tìm và thay chuỗi chính xác. Kiểm tra `includes()` trước khi thay và báo kết quả.

---

## 4. Landing page chiến dịch (Trang tĩnh `/p/<slug>.html`)

**Cấu trúc khuyến nghị:** poster ảnh gốc (rõ nét) → CTA 1 → hero (tiêu đề + ưu đãi + nút gọi/Zalo) → khối ưu đãi (giá gạch, ví dụ ~~250K~~ 0đ) → CTA 2 → đánh giá khách hàng (ảnh thật, có xin phép) → CTA 3 → vì sao chọn chúng tôi → "Cách thức nhận ưu đãi" (3 bước) → khối đặt cọc QR có CTA 4 → bản đồ, TikTok, Fanpage → khối cuối có CTA 5.

- Bọc toàn bộ trong `<div id="lp">` và scope mọi CSS bằng `#lp …`. Biến màu khai báo trên `#lp{--bg:…;--ivory:…;--muted:…;--gold:…}`. Thêm vào theme `.article:has(#lp){max-width:none;padding:0}` để trang được tràn rộng.
- Ảnh: **khách tải ảnh gốc** qua nút "Chèn hình ảnh" của Blogger, agent lấy URL `blogger.googleusercontent.com/...` rồi đổi kích thước sang `/s1600/` hoặc `/s1536/`. Không nhét ảnh base64 lớn vào trang, vì ảnh sẽ mờ và nặng. Blogger tự chèn `<div class="separator">…` khi tải ảnh, nhớ xoá các khối đó.
- **5 nút đăng ký** chia đều từ đầu đến cuối trang: `<a class="btn btn-reg" href="#dang-ky" data-reg="1..5">`. Mỗi nút một câu kêu gọi khác nhau.
- Mọi nút `data-reg` mở cùng một **popup 4 bước** (mẫu ở phần **PHỤ LỤC B**). Popup được chuyển vào `<body>` để luôn nổi trên cùng.

---

## 5. Hệ thống theo dõi (Google Form + Sheets, miễn phí, không cần OAuth)

> Không dùng Apps Script Web App, vì nó đòi cửa sổ cấp quyền OAuth mở thành popup riêng, agent không bấm được và khách thường không tìm thấy. Google Form gửi dữ liệu qua `formResponse` không cần quyền gì.

1. Mở `forms.new`. Tạo câu hỏi **Trả lời ngắn** đầu tiên tên `loai`, đổi loại câu hỏi sang "Trả lời ngắn", rồi dùng nút **Nhân bản** (giữ nguyên loại) và đổi tên lần lượt: `aff, vid, info, ten, sdt, email, gioitinh, tuoi, sangloc, nentang, thietbi`. Không bật "bắt buộc", không thu email.
2. Bấm **Xuất bản**. Vào tab Câu trả lời → **Liên kết với Trang tính** → tạo bảng mới tên "<THUONG_HIEU> - Doi tac (DU LIEU)".
3. Lấy ID: fetch trang `viewform`, đọc `FB_PUBLIC_LOAD_DATA_`:
   ```js
   const t=await (await fetch('https://docs.google.com/forms/d/<EDIT_ID>/viewform')).text();
   const d=JSON.parse(t.match(/FB_PUBLIC_LOAD_DATA_ = (.*?);<\/script>/s)[1]);
   d[1][1].map(q=>q[1]+'='+q[4][0][0]).join(' | ');   // tên=entryId
   // action: /forms/d/e/<FORM_PUBLIC_ID>/formResponse
   ```
4. Đổi tên tab câu trả lời thành **DuLieu** và thêm cột cuối **trangthai** (chủ shop gõ "Đã cọc"). Nếu sau này thêm câu hỏi vào Form, Google tự chèn cột trước `trangthai` và công thức tự dịch theo.
5. Gắn **PHỤ LỤC A** (script theo dõi) vào trang landing, ngay trước khối `DEPOSIT`.

**Các giá trị cột `loai`:** `visit` (mỗi phiên 1 lần), `click` (bấm nút số mấy), `lead` (đăng ký), `paid` (bấm "đã chuyển khoản"), `zalo` (bấm gửi ảnh), `done` (hoàn tất), `share` (bấm chia sẻ, kèm kênh).

### 5.1 Tab DoiTac
A: Mã (viết liền, không dấu) · B: Tên · C: SĐT · D: Hoa hồng mỗi khách đã cọc · E2:
`=ARRAYFORMULA(IF(A2:A="";"";"https://www.<TEN_MIEN>/p/<slug>.html?aff="&UPPER(A2:A)))`

### 5.2 Tab TongHop (B1 = từ ngày, B2 = tới ngày; A4:I4 là tiêu đề)
Locale Việt Nam dùng dấu **`;`** để ngăn đối số. Kiểm tra trước bằng `=SUM(1;2)`.
```
A5 ={"TRUC-TIEP";FILTER(UPPER(DoiTac!A2:A);DoiTac!A2:A<>"")}
B5 =MAP(A5:A;LAMBDA(m;IF(m="";"";IF(m="TRUC-TIEP";"(Khách vào trực tiếp)";IFERROR(INDEX(DoiTac!B:B;MATCH(m;DoiTac!A:A;0));"")))))
C5 (người) =MAP(A5:A;LAMBDA(m;IF(m="";"";IFERROR(ROWS(UNIQUE(FILTER(DuLieu!D:D;DuLieu!B:B="visit";DuLieu!C:C=m;DuLieu!A:A>=$B$1;DuLieu!A:A<$B$2+1)));0))))
D5 (đăng ký) =MAP(A5:A;LAMBDA(m;IF(m="";"";COUNTIFS(DuLieu!B:B;"lead";DuLieu!C:C;m;DuLieu!A:A;">="&$B$1;DuLieu!A:A;"<"&($B$2+1)))))
E5 (tỷ lệ) =MAP(C5:C;D5:D;LAMBDA(c;d;IF(N(c)=0;"";d/c)))
F5 (đã cọc) =MAP(A5:A;LAMBDA(m;IF(m="";"";COUNTIFS(DuLieu!B:B;"lead";DuLieu!C:C;m;DuLieu!<cột trangthai>:<cột trangthai>;"*c?c*";DuLieu!A:A;">="&$B$1;DuLieu!A:A;"<"&($B$2+1)))))
G5 (hoa hồng) =MAP(A5:A;F5:F;LAMBDA(m;f;IF(OR(m="";m="TRUC-TIEP");"";f*SUMIFS(DoiTac!D:D;DoiTac!A:A;m))))
H5 (link) =MAP(A5:A;LAMBDA(m;IF(OR(m="";m="TRUC-TIEP");"";"https://www.<TEN_MIEN>/p/<slug>.html?aff="&m)))
I5 (tổng lượt) =MAP(A5:A;LAMBDA(m;IF(m="";"";COUNTIFS(DuLieu!B:B;"visit";DuLieu!C:C;m;DuLieu!A:A;">="&$B$1;DuLieu!A:A;"<"&($B$2+1)))))
```
⚠️ Không dùng `COUNTUNIQUE(FILTER(...))`, vì khi FILTER rỗng hàm vẫn trả về 1. Dùng `IFERROR(ROWS(UNIQUE(FILTER(...)));0)`.

### 5.3 Tab NenTang (pivot tự động, dùng HSTACK để tránh lỗi dấu phân cách mảng)
```
A4 =IFERROR(QUERY(FILTER(HSTACK(DuLieu!<nentang>2:<nentang>;DuLieu!<thietbi>2:<thietbi>);DuLieu!B2:B="visit";DuLieu!<nentang>2:<nentang><>"";DuLieu!A2:A>=TongHop!$B$1;DuLieu!A2:A<TongHop!$B$2+1);"select Col1, count(Col1) group by Col1 pivot Col2 label Col1 'Nền tảng'";0);"Chưa có dữ liệu")
G4 = như trên với HSTACK(DuLieu!C2:C; cột thietbi)  → đối tác × thiết bị
A20 = như trên với HSTACK(DuLieu!C2:C; cột nentang) → đối tác × nền tảng
```

**Mẹo nhập liệu Google Sheets bằng agent:**

- Ký tự `\t` trong lệnh type **không** chuyển sang ô bên cạnh. Phải gõ từng ô rồi dùng phím `Tab` hoặc `Return`.
- Chữ đầu ô bắt đầu bằng "Đ" đôi khi bị mất do bộ gõ hoặc gợi ý tự động. Kiểm tra lại bằng zoom.
- **Trước khi gõ phải chắc chắn đang ở đúng tab.** Chụp màn hình hoặc xem tên ô. Click tab có thể trượt khi kích thước cửa sổ đổi. Nếu lỡ gõ nhầm vào DuLieu thì dùng `Ctrl+Z` ngay.
- Đọc dữ liệu để kiểm tra (không sửa) bằng: `fetch('/spreadsheets/d/<ID>/gviz/tq?tqx=out:csv&sheet=DuLieu&range=A1:N500&x='+Date.now())`.
- Xoá dòng thử: chọn dòng bằng Name box → chuột phải vào số dòng → "Xóa hàng". Sau đó xác nhận lại bằng gviz.

---

## 6. Link affiliate chống gõ sai (dán vào theme, ngay trước `</head>`)

Khách hay gõ thiếu `?` (ví dụ `…99k.html.affilate=ten`) và Blogger trả về trang trống. Script sau tự chuyển về đúng trang:
```html
<script type='text/javascript'>//<![CDATA[
(function(){var p=location.pathname,m=p.match(/^\/p\/<SLUG>(\.html)?(.*)$/i);if(!m||(m[1]&&!m[2]))return;var r='';try{r=decodeURIComponent(m[2])}catch(e){r=m[2]}var c=(r.match(/=\s*([A-Za-z0-9_-]+)/)||[])[1]||r.replace(/[^A-Za-z0-9_-]/g,'');var q=location.search.replace(/^\?/,'');try{sessionStorage.setItem('hh_ref',document.referrer||'-')}catch(e){}location.replace('/p/<SLUG>.html'+(c?'?aff='+encodeURIComponent(c.toUpperCase())+(q?'&'+q:''):(q?'?'+q:'')));})();
//]]></script>
```
Script theo dõi (Phụ lục A) nhận được nhiều tên tham số: `aff, affiliate, affilate, aff_id, ref, ctv`. Mã đối tác được lưu 30 ngày trên máy khách.

**Link mẫu gửi đối tác:** `https://www.<TEN_MIEN>/p/<slug>.html?aff=MADOITAC&utm_source=zalo` (hoặc `facebook`, `tiktok`). Tham số `utm_source` giúp xác định chắc chắn nền tảng khi khách mở link bằng Chrome hay Safari.

---

## 7. Microsoft Clarity (heatmap miễn phí)

1. Khách tự đăng nhập clarity.microsoft.com bằng Google. Agent chỉ tick ô Terms **sau khi khách nói đồng ý**, và không tick ô nhận email quảng cáo.
2. Tạo project: tên thương hiệu, URL website. Với ngành spa hoặc y tế, chọn ngành "B2C Services" để tránh điều khoản dữ liệu sức khoẻ, trừ khi doanh nghiệp thật sự xử lý dữ liệu y tế.
3. Lấy Project ID trong URL (`/projects/view/<ID>/…`). Dán vào theme trước `</head>`:
```html
<script type="text/javascript">(function(c,l,a,r,i,t,y){c[a]=c[a]||function(){(c[a].q=c[a].q||[]).push(arguments)};t=l.createElement(r);t.async=1;t.src="https://www.clarity.ms/tag/"+i;y=l.getElementsByTagName(r)[0];y.parentNode.insertBefore(t,y);})(window, document, "clarity", "script", "<PROJECT_ID>");</script>
```
4. Kiểm tra: mở trang thật, chạy `typeof window.clarity==='function'`. Dữ liệu hiện sau khoảng 30 phút đến 2 giờ.

---

## 8. Kiểm thử bắt buộc (trước khi bàn giao)

- [ ] Mở `…/p/<slug>.html?aff=TEST` → `HH.aff==='TEST'`, nội dung chuyển khoản có mã. Có đủ 5 nút `data-reg`.
- [ ] Mở link gõ sai `…/p/<slug>.html.affilate=test` → trang tự chuyển đúng.
- [ ] Chạy hết popup 4 bước với dữ liệu "TEST xoa": báo lỗi đúng khi thiếu trường, QR đúng số tiền và nội dung, nút "Hoàn tất" chỉ mở sau khi bấm Zalo.
- [ ] Bảng DuLieu nhận đủ cột (nentang, thietbi, email…). TongHop và NenTang ra số.
- [ ] **Xoá toàn bộ dòng thử**. Xoá `localStorage` (`hh_reg, hh_aff, hh_vid`) và `sessionStorage` trên trình duyệt test.
- [ ] Ảnh poster nét, trang hiển thị đúng ở bề ngang điện thoại.

## 9. Bàn giao (gửi khách bằng tiếng Việt, ngắn gọn)

- Link website, link landing gốc, cách tạo link affiliate (`?aff=MÃ`), link Google Sheets (các tab DoiTac, TongHop, NenTang, DuLieu) và link Clarity.
- Cách đánh dấu "Đã cọc", cách thêm đối tác, cách lọc theo ngày.
- Giới hạn: không tự xác minh tiền về. Lượt chia sẻ chỉ đếm số lần khách bấm nút. Link dán sang trình duyệt thì nền tảng có thể ghi là "không rõ", nên dùng `utm_source`.
- Nhắc: không xoá hay sửa Google Form "Theo dõi", vì đó là đường dữ liệu về bảng.

---

## Áp dụng cho ngành khác

Chỉ cần đổi: nội dung, màu thương hiệu (biến CSS), `CAU_HOI_SANG_LOC` và các lựa chọn của nó, tên ưu đãi, tiền cọc. Ví dụ:

- **Nha khoa:** "Vấn đề răng" (sâu răng, niềng, tẩy trắng, implant…).
- **Gym/Yoga:** "Mục tiêu" (giảm cân, tăng cơ, dẻo dai…).
- **Trung tâm Anh ngữ:** "Trình độ" và "Mục tiêu" (IELTS, giao tiếp…).
- **Bất động sản:** "Nhu cầu" (mua ở, đầu tư) + "Tầm tài chính". Đổi bước cọc thành "Đặt lịch xem nhà", có thể bỏ bước QR.
- **Nhà hàng/khoá học:** "Số người" hoặc "Khung giờ".

Nếu không thu tiền cọc thì bỏ bước 2 và 3 của popup (Chuyển khoản, Gửi ảnh), đi thẳng từ Đăng ký sang Thành công. Nếu ưu đãi không yêu cầu chia sẻ thì bỏ khối `.shr` ở bước 4.

---

## PHỤ LỤC A – Script theo dõi + cấu hình đặt cọc (dán trong `<script>` của trang landing)

Thay các `{{...}}`. Mọi lần gửi đều tự kèm `aff, vid, nentang, thietbi`.
```js
var DEPOSIT_AFF='';
var HH=(function(){var F='https://docs.google.com/forms/d/e/{{FORM_PUBLIC_ID}}/formResponse',E={loai:'entry.{{E_LOAI}}',aff:'entry.{{E_AFF}}',vid:'entry.{{E_VID}}',info:'entry.{{E_INFO}}',ten:'entry.{{E_TEN}}',sdt:'entry.{{E_SDT}}',email:'entry.{{E_EMAIL}}',gioitinh:'entry.{{E_GIOITINH}}',tuoi:'entry.{{E_TUOI}}',sangloc:'entry.{{E_SANGLOC}}',nentang:'entry.{{E_NENTANG}}',thietbi:'entry.{{E_THIETBI}}'};
function g(k){try{return localStorage.getItem(k)}catch(e){return null}}function s(k,v){try{localStorage.setItem(k,v)}catch(e){}}
var q=(function(u){return u.get('aff')||u.get('affiliate')||u.get('affilate')||u.get('aff_id')||u.get('ref')||u.get('ctv')||''})(new URLSearchParams(location.search)).toUpperCase().replace(/[^A-Z0-9_-]/g,'').slice(0,30);
if(q)s('hh_aff',JSON.stringify({c:q,t:Date.now()}));
var a='';try{var o=JSON.parse(g('hh_aff')||'null');if(o&&2592e6>Date.now()-o.t)a=o.c}catch(e){}
a=a||'TRUC-TIEP';
var v=g('hh_vid');if(!v){v=Date.now().toString(36)+Math.random().toString(36).slice(2,8);s('hh_vid',v)}
var UA=navigator.userAgent,RF=((function(){try{var x=sessionStorage.getItem('hh_ref');if(x!==null){sessionStorage.removeItem('hh_ref');return x==='-'?'':x}}catch(e){}return document.referrer||''})()).toLowerCase(),US=((new URLSearchParams(location.search).get('utm_source'))||'').toLowerCase();
var P=(function(){if(/zalo/i.test(UA)||/zalo/.test(RF)||US.indexOf('zalo')>-1)return 'Zalo';
if(/messenger|orca-android/i.test(UA)||/messenger\.com/.test(RF)||US.indexOf('messenger')>-1)return 'Messenger';
if(/instagram/i.test(UA)||/instagram\./.test(RF)||US.indexOf('instagram')>-1)return 'Instagram';
if(/FBAN|FBAV|FB_IAB|FBIOS/i.test(UA)||/facebook\.|fb\.com|fb\.me/.test(RF)||US.indexOf('facebook')>-1||US==='fb')return 'Facebook';
if(/musical_ly|bytedance|tiktok|trill_/i.test(UA)||/tiktok\./.test(RF)||US.indexOf('tiktok')>-1)return 'TikTok';
if(/youtube\.|youtu\.be/.test(RF))return 'YouTube';
if(/google\./.test(RF))return 'Google';
if(/bing\.|coccoc|yahoo\./.test(RF))return 'Tìm kiếm khác';
if(RF&&RF.indexOf(location.hostname)>-1)return 'Website';
if(RF)return 'Web khác ('+RF.split('/')[2]+')';
return 'Trực tiếp / không rõ'})();
var D=/ipad|tablet/i.test(UA)?'Máy tính bảng':(/mobi|android|iphone/i.test(UA)?'Điện thoại':'Máy tính');
var OS=/iphone|ipad/i.test(UA)?'iOS':/android/i.test(UA)?'Android':/windows/i.test(UA)?'Windows':/mac os/i.test(UA)?'macOS':'Khác';
function send(t,x){var b=new URLSearchParams();b.append(E.loai,t);b.append(E.aff,a);b.append(E.vid,v);b.append(E.nentang,P);b.append(E.thietbi,D);for(var k in x)if(E[k])b.append(E[k],x[k]);try{fetch(F,{method:'POST',mode:'no-cors',body:b,keepalive:true})}catch(e){}}
var sk='hh_v_'+a,seen=null;try{seen=sessionStorage.getItem(sk)}catch(e){}
if(!seen){try{sessionStorage.setItem(sk,'1')}catch(e){}send('visit',{info:OS+' | '+(document.referrer||'(không có nguồn)').slice(0,120)})}
if(a!=='TRUC-TIEP')DEPOSIT_AFF=' '+a.replace(/[^A-Z0-9]/g,'');
return{aff:a,vid:v,send:send};})();
var DEPOSIT={bankId:"{{BIN_NGAN_HANG}}",bankName:"{{TEN_NGAN_HANG}}",accountNo:"{{SO_TAI_KHOAN}}",accountName:"{{CHU_TAI_KHOAN_KHONG_DAU}}",amount:{{TIEN_COC_SO}},memo:"{{MA_NOI_DUNG_CK}}"};
DEPOSIT.memo+=DEPOSIT_AFF;
```

## PHỤ LỤC B – Popup đăng ký 4 bước + CSS nút CTA (dán ở cuối nội dung trang landing, sau `</section>` cuối)

- Thay `{{...}}`. Thay danh sách lựa chọn trong `#hhSk` cho phù hợp ngành (hiện là ví dụ ngành spa).
- Đổi màu vàng `#b0894a / #8f6c33 / #c9a05a` theo thương hiệu. Nút CTA dùng biến `--ivory, --bg, --muted` của `#lp`.
- Trang cần có `var DEPOSIT` (Phụ lục A) và các nút `<a class="btn btn-reg" href="#dang-ky" data-reg="N">`.

```html
<style>
#lp .cta-band{padding:clamp(30px,6vw,52px) 20px;text-align:center;background:linear-gradient(180deg,var(--ivory),var(--bg))}
#lp .cta-band p{margin:12px 0 0;color:var(--muted);font-size:14px}
#lp .cta-in{text-align:center;margin:0 0 28px}
#lp .btn-reg{display:inline-flex;align-items:center;justify-content:center;border-radius:999px;text-decoration:none;font-weight:700;letter-spacing:.06em;text-transform:uppercase;background:linear-gradient(135deg,#c9a05a,#8f6c33);color:#fff;font-size:16px;padding:20px 38px;box-shadow:0 12px 28px -12px rgba(143,108,51,.8);animation:hhpulse 2.4s infinite}
#lp .btn-reg:hover{color:#fff}
@keyframes hhpulse{0%,100%{box-shadow:0 0 0 0 rgba(176,137,74,.45),0 12px 28px -12px rgba(143,108,51,.8)}50%{box-shadow:0 0 0 12px rgba(176,137,74,0),0 12px 28px -12px rgba(143,108,51,.8)}}
#hhm{position:fixed;inset:0;z-index:2147483000;display:none;align-items:flex-end;justify-content:center;background:rgba(42,39,36,.6);font-family:"Be Vietnam Pro",system-ui,-apple-system,"Segoe UI",sans-serif;color:#2a2724}
#hhm.open{display:flex}
#hhm *{box-sizing:border-box}
#hhm .box{background:#fff;width:100%;max-width:440px;max-height:94vh;overflow:auto;border-radius:24px 24px 0 0;padding:26px 22px 22px;position:relative;animation:hhup .25s ease-out}
@keyframes hhup{from{transform:translateY(30px);opacity:0}to{transform:none;opacity:1}}
@media(min-width:640px){#hhm{align-items:center}#hhm .box{border-radius:24px;padding:30px 30px 26px}}
#hhm .x{position:absolute;top:10px;right:12px;width:38px;height:38px;border:0;background:#f3ece2;border-radius:50%;font-size:22px;line-height:1;cursor:pointer;color:#6e675e}
#hhm .prog{display:flex;gap:6px;list-style:none;margin:0 44px 18px 0;padding:0;font-size:12px;font-weight:600;color:#bdb4a7}
#hhm .prog li{flex:1;border-top:3px solid #e7ddd0;padding-top:6px}
#hhm .prog li.on{border-color:#b0894a;color:#8f6c33}
#hhm .prog li.ok{border-color:#b0894a;color:#b0894a}
#hhm h3{font:600 27px/1.2 "Cormorant Garamond","Times New Roman",serif;margin:0 0 8px;color:#2a2724}
#hhm h4{font:600 17px/1.35 "Be Vietnam Pro",system-ui,sans-serif;margin:0 0 12px;color:#2a2724}
#hhm .sub{margin:0 0 18px;color:#6e675e;font-size:14.5px;line-height:1.55}
#hhm label{display:block;font-size:13px;font-weight:600;margin:0 0 12px;color:#2a2724}
#hhm input{display:block;width:100%;margin-top:6px;font:16px "Be Vietnam Pro",system-ui,sans-serif;padding:14px 16px;border:1.5px solid #e7ddd0;border-radius:14px;background:#fbf8f4;color:#2a2724;outline:0}
#hhm input:focus{border-color:#b0894a;background:#fff}
#hhm .err{color:#c7685a;font-size:13px;margin:-4px 0 10px}
#hhm .go{display:block;width:100%;margin:6px 0 0;padding:17px 20px;border:0;border-radius:999px;background:linear-gradient(135deg,#c9a05a,#8f6c33);color:#fff;font:700 15px/1 "Be Vietnam Pro",system-ui,sans-serif;letter-spacing:.06em;text-transform:uppercase;cursor:pointer;box-shadow:0 10px 24px -12px rgba(143,108,51,.9)}
#hhm .ghost{flex:1;padding:13px 10px;border:1.5px solid #b0894a;border-radius:999px;background:#fff;color:#8f6c33;font:600 13.5px/1.2 "Be Vietnam Pro",system-ui,sans-serif;cursor:pointer}
#hhm .row2{display:flex;gap:10px;margin-top:10px}
#hhm .note{margin:14px 0 0;font-size:12.5px;color:#6e675e;text-align:center;line-height:1.5}
#hhm a{color:#8f6c33}
#hhm .qr{text-align:center;background:#fbf8f4;border-radius:18px;padding:14px;margin:0 0 14px}
#hhm .qr img{width:230px;max-width:100%;height:auto;display:inline-block}
#hhm dl{display:grid;grid-template-columns:auto 1fr;gap:8px 12px;margin:0 0 14px;font-size:14px}
#hhm dt{color:#6e675e}
#hhm dd{margin:0;font-weight:600;display:flex;align-items:center;gap:8px;flex-wrap:wrap;word-break:break-all}
#hhm dd.amt{color:#c7685a;font-size:17px}
#hhm .cp{border:1px solid #e7ddd0;background:#fff;border-radius:999px;padding:4px 10px;font:600 11px "Be Vietnam Pro",system-ui,sans-serif;color:#8f6c33;cursor:pointer}
#hhm .ok-ic{width:62px;height:62px;border-radius:50%;background:#b0894a;color:#fff;font-size:32px;line-height:62px;text-align:center;margin:4px auto 12px}
#hhm #hhS3,#hhm #hhS4{text-align:center}
#hhm .shr{background:#fbf8f4;border:1px dashed #e6d2ab;border-radius:18px;padding:18px 16px;margin-top:6px}
#hhm .dots{display:flex;justify-content:center;gap:8px;margin:0 0 6px}
#hhm .dots i{width:26px;height:26px;border-radius:50%;border:2px solid #e6d2ab;background:#fff}
#hhm .dots i.f{background:#b0894a;border-color:#b0894a}
#hhm .cnt{margin:0 0 12px;font-size:13px;color:#6e675e}
#hhm .ok2{margin:12px 0 0;color:#8f6c33;font-weight:600;font-size:14px}
#hhm .toast{margin:10px 0 0;font-size:13px;color:#8f6c33}
#hhm .fl{display:block;font-size:13px;font-weight:600;margin:0 0 8px;color:#2a2724}
#hhm .grp{margin:0 0 14px}
#hhm .seg{display:flex;gap:8px}
#hhm .chips{display:flex;flex-wrap:wrap;gap:8px}
#hhm .seg label,#hhm .chips label{margin:0;font-weight:500;font-size:14px;cursor:pointer}
#hhm .seg label{flex:1}
#hhm .seg input,#hhm .chips input{position:absolute;opacity:0;width:1px;height:1px;margin:0;padding:0;border:0;pointer-events:none}
#hhm .seg span,#hhm .chips span{display:block;text-align:center;padding:11px 14px;border:1.5px solid #e7ddd0;border-radius:999px;background:#fbf8f4;color:#2a2724;transition:all .15s}
#hhm .chips span{padding:8px 13px;font-size:13.5px}
#hhm input:checked+span{background:#b0894a;border-color:#b0894a;color:#fff}
#hhm input:focus-visible+span{outline:2px solid #8f6c33;outline-offset:2px}
#hhm select{display:block;width:100%;margin-top:6px;font:16px "Be Vietnam Pro",system-ui,sans-serif;padding:14px 16px;border:1.5px solid #e7ddd0;border-radius:14px;background:#fbf8f4;color:#2a2724;outline:0;-webkit-appearance:none;appearance:none;background-image:linear-gradient(45deg,transparent 50%,#8f6c33 50%),linear-gradient(135deg,#8f6c33 50%,transparent 50%);background-position:calc(100% - 22px) 52%,calc(100% - 16px) 52%;background-size:6px 6px;background-repeat:no-repeat}
#hhm .opt{font-weight:400;color:#6e675e}
#hhm .zalo-big{display:flex;align-items:center;justify-content:center;gap:10px;text-decoration:none;background:#0068ff;color:#fff!important;border-radius:999px;padding:16px;font:700 15px/1 "Be Vietnam Pro",system-ui,sans-serif;margin:4px 0 10px}
#hhm .go[disabled]{opacity:.45;cursor:not-allowed}
#hhm .steps-ol{text-align:left;margin:0 0 16px;padding:14px 16px 14px 34px;background:#fbf8f4;border-radius:16px;font-size:14px;line-height:1.6;color:#2a2724}
#hhm .warn{font-size:13px;color:#c7685a;margin:0 0 12px;text-align:center}
#lp .offer .amount s.old{font-size:.5em;color:var(--muted);margin-right:10px;font-weight:600;vertical-align:middle;text-decoration-thickness:2px}
</style>
<div id="hhm" role="dialog" aria-modal="true" aria-labelledby="hhT"><div class="box">
<button class="x" id="hhX" type="button" aria-label="Đóng">×</button>
<ol class="prog"><li id="hhI1">1. Đăng ký</li><li id="hhI2">2. Chuyển khoản</li><li id="hhI3">3. Gửi ảnh</li><li id="hhI4">4. Thành công</li></ol>
<div id="hhS1"><h3 id="hhT">Đăng ký nhận {{TEN_UU_DAI}}</h3><p class="sub">{{MO_TA_UU_DAI_NGAN}}</p>
<form id="hhF" novalidate>
<label>Số điện thoại / Zalo<input id="hhP" type="tel" inputmode="numeric" maxlength="14" autocomplete="tel" placeholder="VD: 0912 345 678"></label>
<label>Họ và tên<input id="hhN" maxlength="60" autocomplete="name" placeholder="VD: Nguyễn Thu Hà"></label>
<label>Email<input id="hhE" type="email" maxlength="80" autocomplete="email" placeholder="VD: thuha@gmail.com"></label>
<div class="grp"><span class="fl">Giới tính</span><div class="seg"><label><input type="radio" name="hhG" value="Nữ"><span>Nữ</span></label><label><input type="radio" name="hhG" value="Nam"><span>Nam</span></label></div></div>
<label>Độ tuổi<select id="hhA"><option value="">Chọn độ tuổi</option><option>Dưới 18</option><option>18 – 24</option><option>25 – 34</option><option>35 – 44</option><option>45 – 54</option><option>Từ 55 trở lên</option></select></label>
<div class="grp"><span class="fl">{{CAU_HOI_SANG_LOC}} <span class="opt">(chọn một hoặc nhiều)</span></span><div class="chips" id="hhSk"><label><input type="checkbox" value="Da dầu"><span>Da dầu</span></label><label><input type="checkbox" value="Da khô"><span>Da khô</span></label><label><input type="checkbox" value="Da hỗn hợp"><span>Da hỗn hợp</span></label><label><input type="checkbox" value="Da nhạy cảm"><span>Da nhạy cảm</span></label><label><input type="checkbox" value="Mụn"><span>Mụn</span></label><label><input type="checkbox" value="Thâm, nám, tàn nhang"><span>Thâm, nám, tàn nhang</span></label><label><input type="checkbox" value="Lỗ chân lông to"><span>Lỗ chân lông to</span></label><label><input type="checkbox" value="Da xỉn màu"><span>Da xỉn màu</span></label><label><input type="checkbox" value="Lão hóa, nếp nhăn"><span>Lão hóa, nếp nhăn</span></label><label><input type="checkbox" value="Da bình thường"><span>Da bình thường</span></label></div></div>
<p class="err" id="hhErr" hidden></p><button class="go" type="submit">Hoàn thành đăng ký</button></form>
<p class="note">Thông tin chỉ dùng để {{THUONG_HIEU}} tư vấn và xác nhận.</p></div>
<div id="hhS2" hidden><h3>Chuyển khoản đặt cọc</h3><p class="sub">Để hoàn tất đăng ký, quý khách vui lòng <b>chuyển khoản đặt cọc {{TIEN_COC_HIEN_THI}} theo mã QR</b> bên dưới. Mở app ngân hàng, quét mã là số tiền và nội dung đã điền sẵn.</p>
<div class="qr"><img id="hhQr" alt="Mã QR chuyển khoản đặt cọc {{THUONG_HIEU}}" width="230" height="230"></div>
<dl><dt>Ngân hàng</dt><dd id="hhBank"></dd><dt>Số tài khoản</dt><dd><span id="hhAcc"></span><button type="button" class="cp" data-c="hhAcc">Sao chép</button></dd><dt>Số tiền</dt><dd id="hhAmt" class="amt"></dd><dt>Nội dung</dt><dd><span id="hhMemo"></span><button type="button" class="cp" data-c="hhMemo">Sao chép</button></dd></dl>
<p class="warn">Chỉ bấm nút dưới đây sau khi giao dịch đã chuyển thành công.</p><button class="go" id="hhPaid" type="button">Tôi đã chuyển khoản xong</button>
<p class="note">{{GHI_CHU_TIEN_COC}} <a href="#" id="hhBack">Sửa thông tin</a></p></div>
<div id="hhS3" hidden><h3>Gửi ảnh chuyển khoản</h3><p class="sub">Bước cuối cùng: quý khách vui lòng <b>chụp màn hình giao dịch chuyển khoản thành công</b> và gửi vào <b>Zalo {{ZALO_HIEN_THI}}</b> để {{THUONG_HIEU}} xác nhận suất.</p>
<ol class="steps-ol"><li>Chụp màn hình giao dịch thành công trong app ngân hàng.</li><li>Bấm nút Zalo bên dưới, gửi ảnh kèm họ tên của quý khách.</li><li>Quay lại đây và bấm <b>"Tôi đã gửi ảnh"</b>.</li></ol>
<a class="zalo-big" id="hhZalo" href="https://zalo.me/{{ZALO_SO}}" target="_blank" rel="noopener">Mở Zalo gửi ảnh chụp màn hình</a>
<button class="go" id="hhSent" type="button" disabled>Tôi đã gửi ảnh – Hoàn tất</button>
<p class="note" id="hhSentNote">Nút "Hoàn tất" sẽ mở sau khi quý khách bấm gửi ảnh qua Zalo.</p></div>
<div id="hhS4" hidden><div class="ok-ic">✓</div><h3>Đăng ký thành công!</h3><p class="sub">Cảm ơn <b id="hhName"></b> đã đăng ký {{TEN_UU_DAI}} tại {{THUONG_HIEU}}. Chúng tôi sẽ kiểm tra giao dịch và liên hệ xác nhận lịch hẹn trong thời gian sớm nhất.</p>
<div class="shr"><h4>Lưu ý: quý khách vui lòng chia sẻ ưu đãi này cho 5 người bạn thân của mình để hoàn tất điều kiện nhận ưu đãi nhé!</h4><div class="dots" id="hhDots"></div><p class="cnt">Đã chia sẻ <b id="hhShN">0</b>/5</p>
<button class="go" id="hhShare" type="button">Chia sẻ qua Zalo / Messenger</button><div class="row2"><button type="button" class="ghost" id="hhFb">Chia sẻ Facebook</button><button type="button" class="ghost" id="hhCopyL">Sao chép link</button></div><p class="toast" id="hhToast" hidden></p><p class="ok2" id="hhShDone" hidden>Tuyệt vời! Cảm ơn quý khách đã lan tỏa ưu đãi đến bạn bè.</p></div>
<p class="note"><a href="#" id="hhNew">Đăng ký cho người khác</a></p></div>
</div></div>
<script>
(function(){
function $(i){return document.getElementById(i)}
var M,st={};try{st=JSON.parse(localStorage.getItem('hh_reg')||'{}')||{}}catch(e){st={}}
function save(){try{localStorage.setItem('hh_reg',JSON.stringify(st))}catch(e){}}
function track(t,x){try{if(window.HH)HH.send(t,x)}catch(e){}}
function memo(){var d=window.DEPOSIT||{};return (d.memo||'COC')+' '+(st.p||'')}
function copy(t,cb){if(navigator.clipboard&&navigator.clipboard.writeText){navigator.clipboard.writeText(t).then(cb,function(){prompt('Sao chép nội dung:',t)})}else{prompt('Sao chép nội dung:',t)}}
function fillQR(){var d=window.DEPOSIT||{},m=memo();$('hhMemo').textContent=m;$('hhAcc').textContent=d.accountNo||'';$('hhBank').textContent=d.bankName||'';$('hhAmt').textContent=(d.amount||0).toLocaleString('vi-VN')+'đ';
if(d.bankId&&d.accountNo){$('hhQr').src='https://img.vietqr.io/image/'+encodeURIComponent(d.bankId)+'-'+encodeURIComponent(d.accountNo)+'-compact2.png?amount='+(d.amount||'')+'&addInfo='+encodeURIComponent(m)+(d.accountName?'&accountName='+encodeURIComponent(d.accountName):'')}}
function dots(){var c=Math.min(st.sh||0,5),h='';for(var i=0;i!==5;i++)h+='<i class="'+(i>=c?'':'f')+'"></i>';$('hhDots').innerHTML=h;$('hhShN').textContent=c;$('hhShDone').hidden=c!==5}
function show(n){st.step=n;save();[1,2,3,4].forEach(function(i){$('hhS'+i).hidden=i!==n;$('hhI'+i).className=i===n?'on':(n>i?'ok':'')});
if(n===2)fillQR();if(n===3){$('hhSent').disabled=!st.z;$('hhSentNote').hidden=!!st.z}if(n===4){$('hhName').textContent=st.n||'quý khách';dots()}M.querySelector('.box').scrollTop=0}
function open(){M.classList.add('open');document.documentElement.style.overflow='hidden';show(st.p?Math.min(Math.max(st.step||2,2),4):1);if(!st.p)setTimeout(function(){$('hhP').focus()},250)}
function close(){M.classList.remove('open');document.documentElement.style.overflow=''}
function link(){var u=location.origin+location.pathname,a=window.HH&&HH.aff;return a&&a!=='TRUC-TIEP'?u+'?aff='+encodeURIComponent(a):u}
var TXT='{{THUONG_HIEU}} đang có {{TEN_UU_DAI}}. Đăng ký tại đây nhé:';
function shared(ch){st.sh=(st.sh||0)+1;save();dots();track('share',{info:ch,ten:st.n||'',sdt:st.ps||''})}
function toast(t){var e=$('hhToast');e.textContent=t;e.hidden=false;setTimeout(function(){e.hidden=true},2500)}
function init(){M=$('hhm');if(!M||M.dataset.ok)return;M.dataset.ok=1;document.body.appendChild(M);
document.querySelectorAll('[data-reg]').forEach(function(b){b.addEventListener('click',function(e){e.preventDefault();open();track('click',{info:'Nut dang ky '+b.getAttribute('data-reg')})})});
M.addEventListener('click',function(e){if(e.target===M)close()});$('hhX').onclick=close;
document.addEventListener('keydown',function(e){if(e.key==='Escape')close()});
$('hhF').addEventListener('submit',function(e){e.preventDefault();
var p=$('hhP').value.replace(/[^0-9]/g,''),n=$('hhN').value.trim(),em=$('hhE').value.trim(),g=(M.querySelector('input[name=hhG]:checked')||{}).value||'',a=$('hhA').value,sk=[].map.call(M.querySelectorAll('#hhSk input:checked'),function(x){return x.value}).join(', ');
var er='',fo=null;
if(p.length<9||p.length>11){er='Vui lòng nhập đúng số điện thoại.';fo=$('hhP')}
else if(!n){er='Vui lòng nhập họ và tên.';fo=$('hhN')}
else if(!/^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(em)){er='Vui lòng nhập đúng địa chỉ email.';fo=$('hhE')}
else if(!g){er='Vui lòng chọn giới tính.'}
else if(!a){er='Vui lòng chọn độ tuổi.';fo=$('hhA')}
else if(!sk){er='Vui lòng chọn {{CAU_HOI_SANG_LOC_THUONG}}.'}
if(er){$('hhErr').textContent=er;$('hhErr').hidden=false;if(fo)fo.focus();return}
$('hhErr').hidden=true;st={n:n,p:p,ps:p.replace(/^(\d{4})(\d{3})(\d+)$/,'$1 $2 $3'),sh:0};
track('lead',{ten:n,sdt:st.ps,email:em,gioitinh:g,tuoi:a,sangloc:sk});show(2)});
$('hhPaid').onclick=function(){track('paid',{ten:st.n||'',sdt:st.ps||''});show(3)};
$('hhZalo').addEventListener('click',function(){st.z=1;save();$('hhSent').disabled=false;$('hhSentNote').hidden=true;track('zalo',{ten:st.n||'',sdt:st.ps||'',info:'Mo Zalo gui anh'})});
$('hhSent').onclick=function(){if(!st.z)return;track('done',{ten:st.n||'',sdt:st.ps||''});show(4)};
$('hhBack').onclick=function(e){e.preventDefault();$('hhN').value=st.n||'';$('hhP').value=st.p||'';show(1)};
$('hhNew').onclick=function(e){e.preventDefault();st={};save();$('hhF').reset();show(1)};
M.querySelectorAll('.cp').forEach(function(b){b.onclick=function(){copy($(b.getAttribute('data-c')).textContent,function(){b.textContent='Đã chép';setTimeout(function(){b.textContent='Sao chép'},1500)})}});
$('hhShare').onclick=function(){var u=link();if(navigator.share){navigator.share({title:'{{TEN_UU_DAI}} – {{THUONG_HIEU}}',text:TXT,url:u}).then(function(){shared('ung dung')},function(){})}else{copy(TXT+' '+u,function(){toast('Đã sao chép lời mời. Dán vào Zalo hoặc Messenger để gửi cho bạn nhé!')});shared('sao chep')}};
$('hhFb').onclick=function(){window.open('https://www.facebook.com/sharer/sharer.php?u='+encodeURIComponent(link()),'_blank','noopener,width=620,height=560');shared('facebook')};
$('hhCopyL').onclick=function(){copy(TXT+' '+link(),function(){toast('Đã sao chép link. Dán gửi cho bạn bè nhé!')});shared('sao chep link')};
if(location.hash==='#dang-ky')open();}
if(document.readyState==='loading')document.addEventListener('DOMContentLoaded',init);else init();
})();
</script>
```
