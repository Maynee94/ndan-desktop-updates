# NDAN Creator Desktop — bản cập nhật

Repository phân phối công khai cho bộ cài Windows và dữ liệu cập nhật của NDAN Creator Desktop. Không lưu cây mã nguồn dự án, API key, cookie hoặc dữ liệu người dùng tại đây.

## Tải ứng dụng

- [Cài Setup 3.4.3](https://github.com/Maynee94/ndan-desktop-updates/releases/download/v3.4.3/NDAN-Creator-3.4.3-x64-Setup.exe) để nhận cập nhật trong app.
- [Tất cả Releases](https://github.com/Maynee94/ndan-desktop-updates/releases).

Repo nguồn đã Private. Các bản app cũ dùng địa chỉ repo nguồn không thể nhận bản chuyển tiếp từ đó nữa: tải và cài Setup 3.4.3 một lần từ liên kết trên. Dữ liệu và phiên đăng nhập tiếp tục dùng thư mục cũ. Từ 3.4.3, vào Cài đặt > Cập nhật ứng dụng để kiểm tra/tải/cài các bản vá đã phát hành ở repository này.

Bản Portable chạy trực tiếp nhưng không hỗ trợ cập nhật tích hợp.

## Nội dung Release

Chỉ phát hành `.exe`, `.blockmap` và `latest.yml`. Không tải ZIP mã nguồn, AppData, khóa API hoặc phiên đăng nhập lên Releases.

Các bản vá mới được build và kiểm thử trong repo nguồn Private rồi xuất bản qua `DESKTOP_RELEASE_TOKEN`, một Actions secret chỉ có quyền ghi Contents vào repo cập nhật này. Token không được đưa vào app hoặc repository Public. Bản 3.4.3 đã được phát hành thành công qua pipeline này. Workflow import tạm thời đã được bỏ.

Muốn phát hành bản vá mới, tăng version trong package.json/package-lock.json của app và cập nhật nhánh desktop trong repo nguồn. Không ghi đè assets của version đã phát hành. Chủ repo cần gia hạn token trước khi nó hết hạn để pipeline tiếp tục xuất bản.
