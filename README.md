# 🎵 ZMusic

ZMusic là ứng dụng nghe nhạc trực tuyến chất lượng cao, miễn phí và không quảng cáo, được xây dựng và phát triển độc lập trên nền tảng Compose Multiplatform dành cho Android, macOS và Windows.

---

## 📦 Tải xuống & Cài đặt

Người dùng có thể tải các bản dựng chính thức tại:  
🔗 **[GitHub Releases - ZMusic](https://github.com/thangtranne2023/optimize-simpmusic/releases/)**

### 📋 Danh sách file cài đặt trong bản phát hành:

| Nền tảng | File cài đặt | Dung lượng | Ghi chú |
| :--- | :--- | :--- | :--- |
| 📱 Android (Universal) | `ZMusic-universal.apk` | ~56 MB | Tương thích mọi thiết bị Android |
| ⚡ Android (arm64-v8a) | `ZMusic-arm64-v8a.apk` | ~29 MB | Bản tối ưu dung lượng cho smartphone 64-bit |
| 🍏 macOS | `ZMusic-macos.dmg` | ~226 MB | Bộ cài DMG (hỗ trợ cả Apple Silicon & Intel) |
| 🪟 Windows (Setup) | `ZMusic-windows-x64-setup.msix` | ~288 MB | Trình cài đặt chuẩn cho Windows 10/11 x64 |
| 💼 Windows (Portable) | `ZMusic-windows-x64-portable.zip` | ~284 MB | Bản nén chạy trực tiếp, không cần cài đặt |

### 🛠️ Hướng dẫn cài đặt

#### 1. Android
1. Truy cập trang Releases và tải file `.apk` phù hợp (khuyến nghị bản `arm64-v8a` cho các thiết bị đời mới).
2. Mở file APK vừa tải về trên thiết bị.
3. Nếu hệ thống yêu cầu cấp quyền cài đặt từ nguồn ngoài, chọn Cho phép để hoàn tất cài đặt.

#### 2. macOS
1. Tải file `ZMusic-macos.dmg`.
2. Mở file `.dmg` và kéo biểu tượng ZMusic vào thư mục Applications.
3. Trường hợp xuất hiện thông báo bảo mật của macOS (Gatekeeper), vào System Settings > Privacy & Security và chọn Open Anyway để khởi chạy ứng dụng lần đầu.

#### 3. Windows
- Bản cài đặt (.msix): Nhấn đúp vào file `ZMusic-windows-x64-setup.msix` để tiến hành cài đặt vào hệ thống.
- Bản Portable (.zip): Giải nén tệp zip và mở trực tiếp file `ZMusic.exe` để sử dụng ngay mà không cần cài đặt.

---

## ✨ Tính năng nổi bật

- 🎧 Tự động mix nhạc (Auto-Mix & Crossfade): Kích hoạt mặc định ngay khi vừa cài đặt. Tự động nhận diện nhịp điệu (BPM) để chuyển tiếp giữa các bài hát liền mạch, mang phong cách DJ tương tự Apple Music Automix.
- ⚡ Tốc độ phản hồi tức thì: Tối ưu hóa bộ đệm phân tích luồng nhạc, giảm độ trễ khởi động phát bài xuống mức tối thiểu.
- ⏩ Tua nhạc mượt mà không độ trễ: Tận dụng bộ nhớ đệm RAM tốc độ cao, khắc phục hoàn toàn hiện tượng đứng hình hoặc ngắt tiếng khi tua nhanh trên Desktop và thiết bị di động.
- 🎨 Giao diện đa phong cách: Cho phép tùy chọn linh hoạt giữa giao diện hiện đại Spotify Style và giao diện kính mờ cao cấp Apple Music Liquid Glass.
- 🎤 Lời bài hát đồng bộ thời gian thực: Hỗ trợ hiển thị lời bài hát chạy từng từ (Word-by-word), phiên âm đa ngôn ngữ và chế độ hiển thị lời bài hát toàn màn hình.
- 🔐 Đăng nhập Google: Hỗ trợ đồng bộ thư viện nhạc cá nhân, danh sách phát và hiển thị chính xác thông tin tài khoản Google.
- 🎚️ Chất lượng âm thanh trung thực: Tùy chỉnh chất lượng phát trực tuyến và bộ cân bằng âm thanh (Equalizer) tích hợp sẵn với nhiều preset tối ưu cho từng thể loại nhạc.
- 🛡️ Không quảng cáo & Tôn trọng quyền riêng tư: Không chèn quảng cáo bên thứ ba, hỗ trợ chế độ nghe nhạc nền và ngoại tuyến.

---

## 🔒 Kiến trúc phần mềm & Tình trạng bản quyền mã nguồn

- 🛡️ Mã nguồn đóng & Độc lập hoàn toàn (Proprietary & Clean-Room Architecture): ZMusic là sản phẩm phần mềm mã nguồn đóng, được nghiên cứu và viết lại hoàn toàn mới (clean-room rewrite) từ kiến trúc nền tảng đến toàn bộ hệ thống xử lý giao diện và giải mã âm thanh. Ứng dụng không kế thừa, không sao chép và không chứa mã nguồn của SimpMusic.
- ⚖️ Tuân thủ pháp lý & Không xung đột giấy phép (License Compliance): Do toàn bộ mã nguồn được thiết kế và triển khai độc lập, ZMusic hoàn toàn không chịu sự ràng buộc hay nghĩa vụ dẫn xuất từ bất kỳ giấy phép mã nguồn mở nào của các dự án trước đây (bao gồm GPL hoặc các biến thể tương đương).
- 📦 Phân phối nhị phân độc quyền: Toàn bộ mã nguồn cốt lõi được giữ kín và không công khai. Nhóm phát triển chỉ phát hành trực tiếp các gói cài đặt đã được đóng gói và ký duyệt tại trang phát hành chính thức Releases.

---

## 📜 Tuyên bố miễn trừ trách nhiệm (Disclaimer)

- ZMusic được phân phối dưới dạng bản dựng độc lập cho mục đích cá nhân và có thể thương mại trong tương lai.
- Ứng dụng không sở hữu bản quyền đối với bất kỳ nội dung âm thanh hoặc dữ liệu đa phương tiện nào. Mọi luồng phát và dữ liệu liên quan được truy xuất công khai thông qua dịch vụ lưu trữ của YouTube / YouTube Music.
- Vui lòng tôn trọng quyền tác giả và ủng hộ các nghệ sĩ bằng cách sử dụng các dịch vụ bản quyền chính thức.
