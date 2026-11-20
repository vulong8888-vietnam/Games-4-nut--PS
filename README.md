# Retro Player

Chơi game NES (4 nút), Mega Drive (6 nút), SNES, PS1 từ file bạn tải về. Chạy bằng EmulatorJS. Icon app là tay cầm NES.

## Build APK trên GitHub (kéo thả)

1. Giải nén file zip.
2. Tạo repo mới trên GitHub, chọn **uploading an existing file**.
3. Mở thư mục vừa giải nén, chọn **tất cả** file và thư mục bên trong (Ctrl+A), kéo thả vào trang GitHub, rồi bấm **Commit changes**.
   - Trên Mac, thư mục `.github` bị ẩn trong Finder. Bấm Cmd+Shift+. (dấu chấm) để hiện ra trước khi chọn tất cả.
4. Vào tab **Actions**, workflow **Build APK** tự chạy (5 đến 10 phút). Nếu chưa chạy, chọn Build APK rồi bấm **Run workflow**.
5. Xong thì vào mục **Releases** bên phải trang repo, tải `retro-player.apk` về điện thoại, mở file và cài.

### Nếu tab Actions không thấy workflow nào

Nghĩa là thư mục `.github` chưa được tải lên. Làm cách này: bấm **Add file, Create new file**, ở ô tên file gõ `.github/workflows/build-apk.yml`, mở file `build-apk.yml` trong thư mục này, copy toàn bộ nội dung dán vào, bấm **Commit changes**.

### Nếu bước đăng lên Releases báo lỗi 403

Vào Settings, Actions, General, Workflow permissions, chọn **Read and write permissions**, rồi chạy lại workflow.
