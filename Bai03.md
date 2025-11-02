1. Danh sách Stakeholders
| **Stakeholder**                                   | **Vai trò**                                                                     | **Nguồn yêu cầu**                                                        |
| ------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| **Học viên (Student)**                            | Người sử dụng chính, đăng ký, mua và học các khóa học trực tuyến.               | Mong muốn học tập linh hoạt, dễ truy cập, nội dung chất lượng.           |
| **Giảng viên (Instructor)**                       | Cung cấp và quản lý nội dung khóa học, bài giảng, bài tập, kiểm tra.            | Cần công cụ quản lý khóa học, thống kê học viên, tạo bài học dễ dàng.    |
| **Quản trị viên (Admin)**                         | Quản lý người dùng, khóa học, giao dịch, và đảm bảo hệ thống hoạt động ổn định. | Yêu cầu giám sát, bảo mật, và duy trì hiệu năng hệ thống.                |
| **Nhà phát triển hệ thống (Developer)**           | Xây dựng, bảo trì, và mở rộng chức năng hệ thống.                               | Yêu cầu từ người dùng và quản trị viên về tính năng, hiệu năng, bảo mật. |
| **Bộ phận hỗ trợ (Support Staff)**                | Giải quyết vấn đề kỹ thuật, hỗ trợ người dùng khi gặp lỗi hoặc khó khăn.        | Cần hệ thống quản lý yêu cầu hỗ trợ (ticket system).                     |
| **Đối tác thanh toán (Payment Gateway)**          | Xử lý thanh toán trực tuyến (VNPay, Momo, Visa...).                             | Yêu cầu tích hợp API an toàn, chính xác.                                 |
| **Tổ chức kiểm định nội dung (Content Reviewer)** | Kiểm tra và phê duyệt nội dung khóa học trước khi xuất bản.                     | Yêu cầu giao diện duyệt và phản hồi nội dung nhanh chóng.                |

2. Yêu cầu chức năng (Functional Requirements)
| **Mã**  | **Yêu cầu chức năng**    | **Mô tả**                                                                                             |
| ------- | ------------------------ | ----------------------------------------------------------------------------------------------------- |
| **FR1** | Quản lý người dùng       | Hệ thống cho phép đăng ký, đăng nhập, cập nhật thông tin người dùng (học viên, giảng viên, admin).    |
| **FR2** | Quản lý khóa học         | Giảng viên có thể tạo, chỉnh sửa, xóa, và xuất bản khóa học; học viên có thể xem và đăng ký khóa học. |
| **FR3** | Thanh toán khóa học      | Học viên có thể thanh toán qua các cổng thanh toán tích hợp (VNPay, Momo, Visa, COD...).              |
| **FR4** | Quản lý nội dung học tập | Bao gồm video bài giảng, tài liệu PDF, bài tập, bài kiểm tra, và diễn đàn thảo luận.                  |
| **FR5** | Theo dõi tiến độ học tập | Hệ thống lưu lại tiến độ học, điểm số, và kết quả của học viên.                                       |
| **FR6** | Đánh giá và phản hồi     | Học viên có thể đánh giá khóa học và giảng viên, giúp cải thiện chất lượng nội dung.                  |
| **FR7** | Quản lý thông báo        | Gửi thông báo đến học viên (nhắc học, ưu đãi, cập nhật khóa học).                                     |
| **FR8** | Báo cáo và thống kê      | Admin và giảng viên xem báo cáo về doanh thu, lượt đăng ký, hiệu quả học tập.                         |
| **FR9** | Quản lý hỗ trợ           | Hệ thống cung cấp module gửi yêu cầu hỗ trợ và theo dõi trạng thái.                                   |

3. Yêu cầu phi chức năng (Non-functional Requirements)
| **Mã**   | **Yêu cầu phi chức năng**                   | **Mô tả**                                                                          |
| -------- | ------------------------------------------- | ---------------------------------------------------------------------------------- |
| **NFR1** | **Hiệu năng (Performance)**                 | Hệ thống phải phản hồi trong vòng ≤ 3 giây cho 95% yêu cầu người dùng.             |
| **NFR2** | **Bảo mật (Security)**                      | Dữ liệu người dùng và thanh toán phải được mã hóa (HTTPS, SSL/TLS).                |
| **NFR3** | **Khả năng mở rộng (Scalability)**          | Hệ thống hỗ trợ mở rộng người dùng từ 1.000 lên 100.000 mà không gián đoạn.        |
| **NFR4** | **Tính sẵn sàng (Availability)**            | Hệ thống đảm bảo uptime ≥ 99.5% trong năm.                                         |
| **NFR5** | **Khả năng sử dụng (Usability)**            | Giao diện thân thiện, hỗ trợ trên nhiều thiết bị (web, mobile).                    |
| **NFR6** | **Khả năng bảo trì (Maintainability)**      | Mã nguồn được thiết kế module hóa, dễ dàng cập nhật tính năng mới.                 |
| **NFR7** | **Sao lưu và phục hồi (Backup & Recovery)** | Dữ liệu hệ thống được sao lưu hàng ngày, có thể khôi phục trong ≤ 4 giờ khi sự cố. |
| **NFR8** | **Tương thích (Compatibility)**             | Hệ thống chạy tốt trên các trình duyệt phổ biến (Chrome, Firefox, Edge, Safari).   |
