# ♟️ MasterChess - Chess Game App Desktop

Một ứng dụng trò chơi Cờ Vua trên nền tảng desktop được phát triển bằng Windows Presentation Foundation (WPF), mang đến trải nghiệm chơi cờ toàn diện với giao diện trực quan, hệ thống AI thông minh và khả năng đồng bộ dữ liệu đám mây.

🔗 **Kho lưu trữ:** [ChessGameAppDesktop](https://github.com/karasuma-2401/ChessGameAppDesktop.git)

---

## ✨ Tính năng nổi bật

* **Hệ thống Tài khoản & Bảo mật**: Quản lý hồ sơ người chơi với tính năng đăng ký, đăng nhập và khôi phục mật khẩu thông qua mã xác thực OTP an toàn (mật khẩu được mã hóa Bcrypt). 
* **Chế độ chơi đa dạng**:
    * **PvE (Player vs Environment)**: Thi đấu với hệ thống Bot AI nhiều cấp độ (từ Beginner đến Master). 
    * **PvP (Player vs Player)**: Chế độ 2 người chơi cục bộ với tùy chỉnh đồng hồ đếm giờ linh hoạt (Bullet, Blitz, Rapid, Classical). 
* **Hệ thống Giải đố (Puzzles)**: Rèn luyện tư duy thông qua các thử thách thế cờ (Puzzles) có sẵn, bao gồm cả Daily Puzzle và hệ thống gợi ý (Hint) nước đi. 
* **Góc Học Tập (Learn)**: Hỗ trợ đắc lực cho người mới thông qua thư viện hướng dẫn di chuyển quân cờ, video phân tích các thế khai cuộc (Openings) và các bài học tàn cuộc (Endgame/Checkmate).
* **Cá nhân hóa Giao diện**: Tùy chỉnh phong cách bàn cờ, kiểu dáng quân cờ và hỗ trợ chuyển đổi giao diện Sáng/Tối (Light & Dark Mode). 
* **Lưu trữ Đám mây (Cloud Save)**: Đồng bộ hóa tiến trình theo thời gian thực, cho phép tạm ngưng và tiếp tục ván đấu (Resume) từ bất kỳ thiết bị nào. 

---

## 🛠 Công nghệ & Kiến trúc

* **Ngôn ngữ lập trình**: C# 
* **Framework**: .NET 9.0, WPF (tận dụng DirectX để tối ưu hóa hiển thị đồ họa).
* **Cơ sở dữ liệu**: Google Firebase (Realtime Database) sử dụng kiến trúc NoSQL, thay thế cho SQL Server cục bộ nhằm giải quyết bài toán đồng bộ dữ liệu người dùng. 
* **Môi trường phát triển**: Microsoft Visual Studio 2026 

---

## 🧠 Thuật toán AI cốt lõi

Trí tuệ nhân tạo của MasterChess được thiết kế để mang lại độ thử thách thực tế cho người chơi:
* **Minimax (Negamax)**: Thuật toán đệ quy dự đoán kịch bản tương lai dựa trên lý thuyết trò chơi đối kháng tổng bằng không.
* **Cắt tỉa Alpha-Beta (Alpha-Beta Pruning)**: Tối ưu hóa hiệu suất bằng cách loại bỏ các nhánh tính toán không cần thiết, giúp AI duyệt sâu hơn.
* **Move Ordering**: Sắp xếp ưu tiên các nước đi "ăn quân" hoặc "phong cấp" để tăng tốc độ cắt tỉa nhánh. 
* **Hàm Đánh giá tĩnh (Evaluation)**: Chấm điểm thế cờ linh hoạt dựa trên ưu thế vật chất (Material) và bảng kiểm soát vị trí (Piece-Square Tables).

---

## 🚀 Hướng dẫn cài đặt

**Clone repository về máy**:
   ```bash
   git clone [https://github.com/karasuma-2401/ChessGameAppDesktop.git](https://github.com/karasuma-2401/ChessGameAppDesktop.git)
```
---
## 👥 Đội ngũ phát triển 
* **Dự án được phát triển dưới sự hướng dẫn của Giảng viên Nguyễn Thị Xuân Hương tại Trường Đại học Công nghệ Thông tin - Khoa Công nghệ Phần mềm.
  * **Lê Minh Thắng (24521603) - Thiết kế giao diện, Xử lý tương tác người dùng.
  * **Nguyễn Đăng Khánh (24520790) - Lập trình core game, Tích hợp Cloud Database.
  * **Thân Nhật Minh (24521085) - Xây dựng mô hình thuật toán AI, Cấu trúc CSDL. 
