# HACKINTOSH TUTORIALS
Chuỗi bài viết này được mình dịch lại từ 1 số guide của Rehabman cho các bạn yếu tiếng Anh có thể đọc hiểu và thực hiện theo. Minh sẽ dẫn link gốc vào cuối mỗi bài dịch để các bạn có thể tiện so sánh các thuật ngữ tiếng Anh.

## Các file config.plist được Rehabman làm sẵn cho laptop và phương pháp Hotpatch
Những file config này được Rehabman làm riêng cho các dòng laptop phổ biến sử dụng card graphic onbard của Intel.
<br>Link download: https://github.com/RehabMan/OS-X-Clover-Laptop-Config
<br>Tuỳ vào cấu hình máy, các bạn chọn file config.plist cho phù hợp để có thể bước đầu boot vào bộ cài một cách thuận lợi nhất.

## 1. Tạo bộ cài macOS lên USB
Thông thường bộ cài macOS được tạo trực tiếp trên môi trường macOS. Một số trường hợp bạn không thể mượn được bạn bè máy Mac hoặc máy Hackintosh có sẵn thì phải tạo bộ cài trên Windows.

Link bài viết chi tiết:

## 2. Cài macOS lên ổ cứng
Sau khi tạo xong USB cài đặt, thêm các kext cần thiết, chúng ta bắt đầu vào giai đoạn cài macOS lên ổ cứng.
Nội dung
- Chia phân vùng trên ổ cứng
- Setup BIOS
- Thực hiện cài đặt macOS

Link bài viết chi tiết:

## 3. Cài Clover Bootloader lên ổ cứng
Mỗi lần boot vào mac phải dùng USB mồi rất bất tiện, vì thế chúng ta cần cài đặt Clovẻ lên ổ cứng để tiện cho việc dual boot.
Mục này chúng ta sẽ đi vào cách cài Clover và thêm boot option cho 1 số máy không hỗ trợ chỉnh sửa trong BIOS.

Link bài viết chi tiết:

## 4. Patch DSDT/SSDT
Có 2 phương pháp patch DSDT/SSDT đó là Static Patch và Hotpatch.

Hotpatch là kĩ thuật patch nóng các bảng DSDT + SSDT khi Clover khởi động, thay cho việc nạp file DSDT + SSDT đã patch sẵn (static patch). Static patch thì có ưu điểm là dễ patch và khó bị lỗi hơn, nhưng mỗi khi update BIOS thì thường là phải patch lại. Còn hotpatch khó thực hiện hơn (nhất là với patch pin), dễ gặp lỗi nếu không cẩn thận, nhưng do patch nóng nên update BIOS thoải mái patch vẫn chạy ngon. Ngoài ra hotpatch nếu tách ra làm nhiều file thì có thể bật/tắt các patch tùy ý, thay vì như 1 file DSDT chứa nhiều patch. Một lợi điểm khác là hotpatch dễ phân phối và áp dụng lên nhiều máy có cấu hình giống hoặc tương tự nhau.
