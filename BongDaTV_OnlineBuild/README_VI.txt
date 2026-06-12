BÓNG ĐÁ TV - Android TV WebView Project

File này là project Android Studio, dùng WebView để mở app HTML nội bộ.

Cách dùng:
1. Giải nén file ZIP.
2. Mở Android Studio.
3. Chọn Open, mở thư mục BongDaTV_Project.
4. Chờ Gradle sync xong.
5. Vào app/src/main/assets/channels.json.
6. Thay URL mẫu bằng link stream/website hợp pháp mà bạn có quyền sử dụng.
7. Build APK:
   Build > Build Bundle(s) / APK(s) > Build APK(s)
8. Cài file app-debug.apk lên Android TV.

Vị trí file chính:
- app/src/main/assets/Bongda.html
- app/src/main/assets/channels.json
- app/src/main/java/com/long/bongdatv/MainActivity.java

Lưu ý:
- Project này KHÔNG giúp vượt chặn mạng/domain. Nếu một website bị mạng hoặc TV chặn thì app WebView cũng có thể không mở được.
- Nếu muốn cập nhật link mà không build lại APK, nên đưa file channels.json lên hosting online rồi sửa HTML để fetch URL online đó.
- Tôi đã để URL mẫu trong channels.json. Hãy chỉ dùng nguồn hợp pháp/có quyền sử dụng.
