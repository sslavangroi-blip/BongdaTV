CÁCH BUILD APK ONLINE KHÔNG CẦN ANDROID STUDIO

Cách này dùng GitHub Actions để tự build APK online.

Bước 1: Tạo tài khoản GitHub nếu chưa có.
Bước 2: Tạo repository mới, ví dụ: BongDaTV.
Bước 3: Upload toàn bộ nội dung trong thư mục BongDaTV_OnlineBuild lên repository.
        Lưu ý: upload các file/folder bên trong, không upload nguyên thư mục mẹ.
Bước 4: Vào tab Actions trên GitHub.
Bước 5: Chọn workflow "Build Android TV APK".
Bước 6: Bấm "Run workflow".
Bước 7: Chờ build xong, kéo xuống phần Artifacts.
Bước 8: Tải file "BongDaTV-debug-apk" về, giải nén ra sẽ có app-debug.apk.
Bước 9: Gửi app-debug.apk sang Android TV bằng USB hoặc Send Files to TV để cài.

SỬA LINK
- Nếu muốn sửa link trước khi build APK: mở app/src/main/assets/channels.json rồi thay URL.
- Sau khi sửa, GitHub Actions sẽ tự build lại khi bạn push/update file.

LƯU Ý QUAN TRỌNG
- Project này chỉ là WebView/HTML app cho Android TV.
- App không giúp vượt chặn mạng hoặc vượt chặn domain.
- Chỉ dùng link/nguồn phát mà bạn có quyền sử dụng hợp pháp.
