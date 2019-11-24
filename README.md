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

Static patch là phương pháp patch cũ trước đây, yêu cầu người chơi hack phải nắm được một số kiến thức nhất định và phải dump file DSDT/SSDT trực tiếp từ hệ thống và chỉnh sửa chúng. Việc sử dụng phương pháp này khiến chúng ta không được phép cập nhật hay thay đổi phiên bản BIOS vì sẽ gây ra lỗi.

Ngược lại, hotpatch ngày nay là 1 phương pháp patch DSDT phổ biến, có thể dùng chung được nhiều máy, update/downgrade BIOS thoải mái mà không sợ gây ra lỗi.
