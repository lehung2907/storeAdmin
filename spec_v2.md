# Đặc tả yêu cầu hệ thống quản lý bán hàng

## 1. Yêu cầu gốc từ khách hàng

### 1.1. Các tính năng ưu tiên
1. **Hệ thống tích điểm và phân hạng thành viên**
   - Tự động tích điểm sau mỗi đơn hàng thanh toán
   - Nhiều mốc hạng thành viên khác nhau
   - Phân hạng khách hàng theo thời gian thực
   - Tự động cập nhật hạng dựa trên tổng điểm

2. **Quản lý hoá đơn tạm**
   - Tạo hoá đơn tạm và gửi cho khách xem
   - Chờ khách xác nhận và thanh toán
   - Nhân viên xác nhận thanh toán trên hệ thống
   - Hệ thống tự động tích điểm và ghi nhận doanh thu

### 1.2. Các tính năng cơ bản
1. **Quản lý hàng hoá**
   - Nhập hàng cho từng cửa hàng
   - Xem danh sách và số lượng tồn kho
   - Tạo và quản lý sản phẩm mới
   - Phân loại và tìm kiếm sản phẩm theo danh mục

2. **Báo cáo và thống kê**
   - Báo cáo bán hàng theo nhân viên
   - Thống kê doanh thu
   - Theo dõi hiệu suất bán hàng

3. **Quản lý cửa hàng**
   - Hỗ trợ nhiều cửa hàng
   - Quản lý riêng biệt cho từng cửa hàng
   - Tổng hợp dữ liệu toàn hệ thống

4. **Phân quyền người dùng**
   - Tạo và quản lý tài khoản nhân viên
   - Phân quyền chi tiết theo chức năng
   - Kiểm soát truy cập thông tin

## 2. Chi tiết cần làm rõ

### 2.1. Hệ thống tích điểm và phân hạng thành viên
- [ ] Xác định cụ thể các mốc hạng thành viên (Ví dụ: Đồng, Bạc, Vàng, Kim Cương...)?
- [ ] Quyền lợi của từng hạng thành viên?
- [ ] Tỷ lệ quy đổi điểm (Ví dụ: 1đ = 1.000đ hay tỷ lệ khác?)?
- [ ] Thời hạn của điểm tích lũy?
- [ ] Chính sách đổi điểm lấy quà?

### 2.2. Quản lý hoá đơn tạm
- [ ] Quy trình xử lý hoá đơn tạm
  - Tạo hoá đơn tạm
  - Gửi cho khách xem
  - Khách xác nhận và thanh toán
  - Nhân viên xác nhận trên hệ thống
  - Hệ thống tự động cập nhật trạng thái

### 2.3. Quản lý hàng hoá
- [ ] Thông tin sản phẩm cần thiết
  - Mã sản phẩm
  - Tên sản phẩm
  - Giá bán
  - Số lượng
  - Đơn vị tính
  - Thông tin khác

- [ ] Phân loại sản phẩm
  - Cấu trúc danh mục sản phẩm (ví dụ: Quần, Áo, Phụ kiện...)?
  - Quản lý danh mục con (ví dụ: Quần jean, Quần kaki, Quần short...)?
  - Tìm kiếm và lọc theo danh mục
  - Báo cáo theo danh mục

- [ ] Quy trình nhập hàng?

### 2.4. Báo cáo và thống kê
- [ ] Các loại báo cáo cần thiết
  - Doanh số
  - Sản phẩm bán chạy
  - Lợi nhuận
  - Báo cáo khác?
- [ ] Tần suất báo cáo (hàng ngày, tuần, tháng)?
- [ ] Các chỉ số KPI cần theo dõi?

### 2.5. Quản lý cửa hàng
- [ ] Quản lý doanh số riêng cho từng cửa hàng?
- [ ] Báo cáo tổng hợp toàn hệ thống?
- [ ] Quy trình chuyển hàng giữa các cửa hàng?

### 2.6. Phân quyền người dùng
- [ ] Danh sách các role trong hệ thống? có bao nhiêu role ?
- [ ] Chi tiết quyền hạn của từng role?
- [ ] Quy trình tạo và quản lý tài khoản?
- [ ] Yêu cầu về xác thực (2FA, OTP...)?

### 2.7. Yêu cầu kỹ thuật
1. **Hiệu năng hệ thống**
   - [ ] Số lượng người dùng đồng thời tối đa?
   - [ ] Thời gian phản hồi của hệ thống?
   - [ ] Khả năng mở rộng (scalability)?

2. **Backup và khôi phục**
   - [ ] Tần suất backup?
   - [ ] Phương thức backup (full/incremental)?
   - [ ] Thời gian lưu trữ backup?
   - [ ] Quy trình khôi phục dữ liệu?
   - [ ] Vị trí lưu trữ backup?

3. **Cơ sở dữ liệu**
   - [ ] Loại database sử dụng?
   - [ ] Cấu trúc database?
   - [ ] Quy mô dữ liệu dự kiến?
   - [ ] Chiến lược phân vùng dữ liệu?

4. **Hosting và triển khai**
   - [ ] Môi trường triển khai (cloud/on-premise)?
   - [ ] Yêu cầu về tài nguyên server?
   - [ ] Chiến lược load balancing?
   - [ ] CDN và caching?

5. **Phát triển**
   - [ ] Công nghệ sử dụng (frontend/backend)?
   - [ ] Quy trình phát triển (DevOps)?
   - [ ] Quản lý phiên bản?
   - [ ] Testing strategy?

### 2.8. Giao diện người dùng
- [ ] Yêu cầu về UI/UX?
- [ ] Responsive design?
- [ ] Hỗ trợ đa ngôn ngữ?
- [ ] Theme và branding?

### 2.9. Triển khai và hỗ trợ
- [ ] Thời gian triển khai dự kiến?
- [ ] Yêu cầu về training?
- [ ] Yêu cầu về hỗ trợ sau triển khai? 