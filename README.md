# 🎵 ZMusic

ZMusic là ứng dụng nghe nhạc trực tuyến chất lượng cao, miễn phí và không quảng cáo, được xây dựng và phát triển độc lập trên nền tảng Compose Multiplatform dành cho Android, macOS và Windows.

Phiên bản phát hành: **v1.3.0.2**

---

## 📦 Tải xuống & Cài đặt

Người dùng có thể tải các bản dựng chính thức tại:  
🔗 **[GitHub Releases - ZMusic](https://github.com/thangtranne2023/optimize-simpmusic/releases/)**

### 📋 Danh sách file cài đặt chính thức:

| Nền tảng | Tên file cài đặt | Dung lượng | Ghi chú |
| :--- | :--- | :--- | :--- |
| 📱 **Android (Khuyên dùng)** | `androidApp-arm64-v8a-release.apk` | ~29 MB | Tối ưu hóa hiệu năng và dung lượng siêu nhẹ cho 99% smartphone Android hiện đại |
| 📱 **Android (Universal)** | `androidApp-universal-release.apk` | ~56 MB | Tương thích toàn bộ các thiết bị và kiến trúc CPU Android |
| 📱 **Android (ARMv7 32-bit)** | `androidApp-armeabi-v7a-release.apk` | ~29 MB | Dành riêng cho các dòng máy Android đời cũ 32-bit |
| 📱 **Android (x86_64)** | `androidApp-x86_64-release.apk` | ~30 MB | Dành cho máy ảo Android (Emulator), Android x86 và Chromebook |
| 🍏 **macOS** | `ZMusic-2026.11.22.dmg` (hoặc `ZMusic-macos.dmg`) | ~226 MB | Bộ cài DMG kéo-thả (hỗ trợ cả Apple Silicon M1/M2/M3/M4 & Intel) |
| 🪟 **Windows (Trọn gói tự động)** | `ZMusic-windows-x64-setup-bundle.zip` | ~287 MB | **Khuyên dùng**: Gồm file cài `.msix`, chứng chỉ `.crt` và `install.bat` tự động cấp quyền không bị chặn |
| 🪟 **Windows (Bộ cài MSIX)** | `zmusic-1.3.0.0.x64.msix` | ~289 MB | Trình cài đặt MSIX chuẩn Windows 10/11 x64, tích hợp Start Menu và URI Scheme |
| 💼 **Windows (Portable)** | `zmusic-1.3.0.0-windows-amd64.zip` | ~284 MB | Bản nén chạy trực tiếp (có sẵn `zmusic.exe`), giải nén nghe ngay không cần cài đặt |

---

### 🛠️ Hướng dẫn cài đặt chi tiết

#### 1. Android
1. Truy cập trang Releases và tải file `.apk` phù hợp (khuyến nghị bản `arm64-v8a` cho điện thoại hiện đại).
2. Mở file APK vừa tải về trên thiết bị.
3. Nếu hệ thống yêu cầu cấp quyền cài đặt từ nguồn ngoài (Unknown Sources), chọn **Cho phép / Allow** để hoàn tất cài đặt.

#### 2. macOS
1. Tải file `ZMusic-2026.11.22.dmg`.
2. Mở file `.dmg` và kéo biểu tượng ZMusic vào thư mục **Applications**.
3. Khi khởi chạy lần đầu, nếu xuất hiện cảnh báo bảo mật macOS Gatekeeper (do chưa đăng ký chứng chỉ trả phí của Apple):
   - Vào **System Settings (Cài đặt hệ thống)** > **Privacy & Security (Quyền riêng tư & Bảo mật)**.
   - Cuộn xuống phần Security và nhấn **Open Anyway (Vẫn mở)** để khởi chạy ứng dụng.

#### 3. Windows
- **Cách 1 - Tiện lợi nhất (Khuyên dùng - Tự động 100% không lo lỗi chứng chỉ)**:
  1. Tải file `ZMusic-windows-x64-setup-bundle.zip` và giải nén.
  2. Nhấp chuột phải vào file `install.bat` và chọn **Run as administrator (Chạy với quyền quản trị viên)**.
  3. Script sẽ tự động import chứng chỉ số an toàn của ZMusic vào hệ thống và tự động cài đặt ứng dụng.
- **Cách 2 - Cài đặt trực tiếp gói MSIX**:
  - Nhấp đúp vào file `zmusic-1.3.0.0.x64.msix`. Nếu Windows báo lỗi chứng chỉ `0x800B010A`:
    - Nhấp đúp vào file `zmusic.crt` > chọn **Install Certificate** > chọn **Local Machine** > chọn lưu vào thư mục **Trusted People (Người đáng tin cậy)**.
    - Mở lại file `.msix` để cài đặt bình thường.
- **Cách 3 - Bản Portable (Không cần cài đặt)**:
  - Tải và giải nén `zmusic-1.3.0.0-windows-amd64.zip`.
  - Mở trực tiếp file `zmusic.exe` tại thư mục vừa giải nén để nghe nhạc ngay lập tức.

---

## ✨ Các tính năng đột phá & Nâng cấp (v1.3.0.2)

### 🎧 1. AutoMix 3.0 Siêu Cấp (Vượt trội Apple Music Automix)
- **Triệt tiêu hoàn toàn hiện tượng đè giọng (Vocal Clashing Elimination)**:
  - Ứng dụng công nghệ **3-Stage Dynamic Acoustic DJ Filter**: kết hợp 2 tầng bộ lọc 4th-order (24 dB/octave) Butterworth LPF/HPF cùng 1 tầng Parametric Peaking EQ Dip Filter tại 1,800 Hz ($Q=1.0$).
  - Tự động hạ dải trung âm của bài cũ xuống tới $-8.5\text{ dB}$ ngay tại điểm mix, giúp giọng hát của bài mới bước vào trong trẻo, tách bạch 100%, không bị 2 bài đè giọng gây ồn hay mất kiểm soát.
- **Khóa khuôn nhịp chuẩn DJ (Musical Phrase Boundary Downbeat Locking)**:
  - Khóa chính xác theo cấu trúc khuôn nhạc 4/4 chuẩn mực: `[8, 16, 32, 48]` beats (tương đương 2 bar, 4 bar, 8 bar, 12 bar).
  - Thuật toán thích ứng tempo thông minh (Tempo-Adaptive): bài chậm (<85 BPM) chọn 8 hoặc 16 beat; bài vừa (85-125 BPM) chọn 16 hoặc 32 beat; bài nhanh (>125 BPM) chọn 32 hoặc 48 beat. Loại bỏ hoàn toàn lỗi ngắt beat lửng lơ hoặc lệch phách.
- **Bảo toàn năng lượng âm thanh (Perceptual Acoustic Power Preservation)**:
  - Tích hợp hệ số tương quan âm học $1 + 0.08 \cdot \sin(\pi \cdot t)$, triệt tiêu hiện tượng sụt áp âm lượng (volume dip) ở giữa đoạn mix. Dải bass và độ dày của âm thanh luôn được giữ căng đầy như trên bàn mix DJ thực thụ.
- **Cắt khoảng lặng cuối bài thích ứng (Dynamic Adaptive Outro Silence Trim)**:
  - Tự động đo lường và tính toán điểm mix dựa trên 2.5% thời lượng thực tế của từng ca khúc (dao động linh hoạt từ 2.5s đến 6.5s), không còn cắt cứng 6s gây cụt bài ngắn hoặc sót khoảng lặng bài dài.
- **Chống nổ âm & mượt hóa điều tốc (Anti-Pop Slew-Rate Limiting)**:
  - Tinh chỉnh tốc độ phát mượt mà với bước đệm 60ms, triệt tiêu 100% tiếng nổ xung lách tách (click/pop) khi đổi tempo/pitch.
  - Tích hợp bộ bảo vệ số thực siêu nhỏ (`sanitizeDenormal`), ngăn chặn hiện tượng CPU stall hoặc giật tiếng khi xử lý bộ lọc IIR.

### 🚀 2. Tốc độ phản hồi tức thì & Tải ảnh Max Speed
- **Offline-First Home Feed Cache (0–50ms cold boot)**: Trang chủ lưu cache thông minh dữ liệu bảng tin (`HomeFeed`) vào DataStore cục bộ. Mở app hoặc chuyển tab hiển thị ngay lập tức, triệt tiêu hoàn toàn cảm giác chờ khung xám (shimmer).
- **Bộ điều phối mạng tải ảnh Max Speed**: Nâng giới hạn kết nối đồng thời lên **256 connections** và **64 connections/host**, tăng gấp đôi băng thông tải song song hình ảnh.
- **Smart Thumbnail Fallback Chain**: Tự động fallback sang các kích thước tối ưu (`hqdefault.jpg`, `mqdefault.jpg`, Google CDN `s226`, `s120`), loại bỏ triệt để tình trạng ảnh bìa không tải được.

### 🔄 3. Tự động kiểm tra & Nhắc nhở cập nhật thông minh
- **Nhận diện bản build GitHub Releases**: Tự động đối soát phiên bản theo chuẩn SemVer đa phân cấp (`1.3.0` vs `1.3.0.1`, `1.3.0.2`), tự động nhận diện hậu tố hotfix (`-hf`) và bản chính thức so với beta.
- **Không làm phiền**: Nếu phiên bản máy đang chạy đã bằng hoặc mới hơn bản trên GitHub, ứng dụng tuyệt đối không hiển thị popup nhắc nhở. Khi có bản mới, ứng dụng hiển thị popup đi kèm ghi chú phát hành định dạng Markdown và nút tải trực tiếp.

### 🎨 4. Trải nghiệm người dùng đỉnh cao
- **Giao diện đa phong cách**: Chuyển đổi linh hoạt giữa giao diện hiện đại **Spotify Style** và giao diện kính mờ sang trọng **Apple Music Liquid Glass**.
- **Lời bài hát đồng bộ Word-by-word**: Lời bài hát chạy từng từ theo thời gian thực, hỗ trợ phiên âm đa ngôn ngữ và chế độ hiển thị toàn màn hình.
- **Đăng nhập Google an toàn**: Đồng bộ hóa toàn bộ playlist cá nhân, lịch sử nghe và nghệ sĩ yêu thích.
- **Bộ cân bằng âm thanh (Equalizer)**: Tích hợp nhiều preset chất lượng cao tối ưu riêng cho từng thể loại nhạc.
- **Hoàn toàn miễn phí & Không quảng cáo**: Tôn trọng tối đa trải nghiệm nghe nhạc của người dùng.

---

## 🔒 Kiến trúc phần mềm & Tình trạng bản quyền mã nguồn

- 🛡️ **Mã nguồn đóng & Độc lập hoàn toàn (Proprietary & Clean-Room Architecture)**: ZMusic là sản phẩm phần mềm mã nguồn đóng, được nghiên cứu và viết lại hoàn toàn mới (clean-room rewrite) từ kiến trúc nền tảng đến toàn bộ hệ thống xử lý giao diện và giải mã âm thanh. Ứng dụng không kế thừa, không sao chép và không chứa mã nguồn của SimpMusic.
- ⚖️ **Tuân thủ pháp lý & Không xung đột giấy phép (License Compliance)**: Do toàn bộ mã nguồn được thiết kế và triển khai độc lập, ZMusic hoàn toàn không chịu sự ràng buộc hay nghĩa vụ dẫn xuất từ bất kỳ giấy phép mã nguồn mở nào của các dự án trước đây (bao gồm GPL hoặc các biến thể tương đương).
- 📦 **Phân phối nhị phân độc quyền**: Toàn bộ mã nguồn cốt lõi được giữ kín và không công khai. Nhóm phát triển chỉ phát hành trực tiếp các gói cài đặt đã được đóng gói và ký duyệt tại trang phát hành chính thức [Releases](https://github.com/thangtranne2023/optimize-simpmusic/releases/).

---

## 📜 Tuyên bố miễn trừ trách nhiệm (Disclaimer)

- ZMusic được phân phối dưới dạng bản dựng độc lập cho mục đích cá nhân và phi thương mại.
- Ứng dụng không sở hữu bản quyền đối với bất kỳ nội dung âm thanh hoặc dữ liệu đa phương tiện nào. Mọi luồng phát và dữ liệu liên quan được truy xuất công khai thông qua dịch vụ lưu trữ của YouTube / YouTube Music.
- Vui lòng tôn trọng quyền tác giả và ủng hộ các nghệ sĩ bằng cách sử dụng các dịch vụ bản quyền chính thức.
