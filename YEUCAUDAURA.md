- **Phần 1. Phân tích:** Mô tả sơ đồ cây cấu trúc Heading cho file SRS.
- 1. Giới thiệu

1.1. Mục đích tài liệu

1.2. Phạm vi hệ thống ("Lớp học ảo")

2. Tổng quan tính năng

2.1. Mô tả chung về lớp học trực tuyến

2.2. Đối tượng sử dụng (Giảng viên, Sinh viên, Quản trị viên)

3. Yêu cầu chức năng (Functional Requirements)

3.1. Quản lý phòng học trực tuyến (Tạo, bắt đầu, kết thúc phòng)

3.2. Quản lý tương tác thời gian thực (Micro, Camera, Chia sẻ màn hình)

3.3. Tính năng điểm danh và theo dõi chuyên cần tự động

4. Yêu cầu giao diện & Trải nghiệm người dùng (UI/UX)

4.1. Giao diện phòng học chính (Bố cục 3 vùng)

4.2. Bảng điều khiển dành cho giảng viên

5. Xử lý lỗi & Ngoại lệ hệ thống

5.1. Xử lý mất kết nối mạng đột ngột

5.2. Mã lỗi và thông báo trạng thái

- **Phần 2. Triển khai:** File báo cáo hoàn chỉnh.

- **Phần 3. Kiểm thử:** Nếu lọc sinh viên theo tên nhưng không ra kết quả (dù nhìn thấy tên đó), hãy trình bày cách dùng hàm TRIM để xử lý.
- Khi sử dụng bộ lọc AutoFilter hoặc hàm tìm kiếm trên Excel, nếu bạn nhìn thấy tên sinh viên nhưng hệ thống lại không trả về kết quả, nguyên nhân thường do khoảng trắng thừa (trailing/leading spaces) bị ẩn ở đầu hoặc cuối chuỗi ký tự.

Cách khắc phục:

Tạo một cột phụ trợ bên cạnh bảng dữ liệu gốc.

Sử dụng hàm =TRIM(ô_dữ_liệu_gốc) để tự động cắt bỏ toàn bộ các khoảng trắng thừa.

Sao chép kết quả đã làm sạch, chọn vùng dữ liệu cũ rồi nhấn Paste Values để ghi đè dữ liệu chuẩn vào hệ thống, sau đó thực hiện lọc lại bình thường.
