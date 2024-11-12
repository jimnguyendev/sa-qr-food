## Quản lý quán ăn - Gọi món bằng QR Code

### Bối cảnh

Hiện nay, nhiều quán ăn, cafe và nhà hàng đang gặp phải các vấn đề như:

- Quy trình gọi món phức tạp, tốn nhiều thời gian.
- Khách hàng phải chờ đợi lâu để nhận được món ăn.
- Nhân viên phục vụ gặp khó khăn trong việc ghi chép, truyền đạt đơn hàng.
- Không có thông tin về tình trạng đơn hàng.

Để giải quyết các vấn đề này, việc ứng dụng công nghệ trong quy trình gọi món trở nên cấp thiết.

### Mục tiêu

Xây dựng một hệ thống cho phép khách hàng tự do lựa chọn và gọi món thông qua mã QR, giúp cải thiện trải nghiệm khách hàng, tối ưu hóa quy trình hoạt động của quán ăn.

### Phạm vi

Hệ thống được thiết kế để áp dụng cho các quán ăn, cafe, nhà hàng với các tính năng chính:

- Cho phép khách hàng tự gọi món thông qua mã QR.
- Hiển thị menu, giá cả và thời gian chờ đợi.
- Giúp nhân viên quản lý đơn hàng dễ dàng.

### Phương pháp khảo sát

Để hiểu rõ về hoạt động hiện tại của quán ăn và nhu cầu của các bên liên quan, chúng tôi đã tiến hành:

1. **Quan sát trực tiếp**: Quan sát quy trình gọi món, nhận món và thanh toán tại các quán ăn.
2. **Phỏng vấn**: Phỏng vấn quản lý, nhân viên phục vụ và một số khách hàng thường xuyên.
3. **Thu thập tài liệu**: Thu thập các tài liệu, quy trình hiện tại của quán ăn.

### Kết quả khảo sát

Dựa trên kết quả khảo sát, chúng tôi đã xác định được các vấn đề và nhu cầu chính như sau:

#### Vấn đề hiện tại

- **Quy trình gọi món phức tạp**: Khách hàng phải gọi phục vụ, phục vụ ghi chép vào phiếu và chuyển bếp. Khách đợi thức ăn, phục vụ mang ra.
- **Thời gian chờ đợi dài**: Khách hàng phải chờ đợi lâu để nhận được món ăn.
- **Sai sót trong ghi chép và truyền đạt**: Nhân viên phục vụ thường mắc lỗi khi ghi chép và truyền đạt đơn hàng.
- **Thiếu thông tin về tình trạng đơn hàng**: Khách hàng không thể theo dõi tình trạng đơn hàng của mình.

#### Nhu cầu của khách hàng

- **Tự do lựa chọn và gọi món**: Khách hàng muốn có thể tự do lựa chọn và gọi món mà không cần phải gọi phục vụ.
- **Theo dõi tình trạng đơn hàng**: Khách hàng muốn biết được tình trạng đơn hàng của mình.

#### Nhu cầu của nhân viên

- **Giảm tải công việc ghi chép, truyền đạt**: Nhân viên mong muốn được giảm bớt các công việc ghi chép và truyền đạt đơn hàng.
- **Quản lý đơn hàng dễ dàng hơn**: Nhân viên cần có công cụ để quản lý đơn hàng một cách hiệu quả hơn.

### Ràng buộc

- **Chi phí triển khai hạn chế**: Giải pháp cần phải phù hợp với ngân sách của quán ăn.
- **Dễ sử dụng**: Giải pháp phải dễ sử dụng, đáp ứng được nhu cầu của cả khách hàng và nhân viên, kể cả những người không quen với công nghệ.


## Phân tích yêu cầu

Được rồi, dưới đây là cách viết yêu cầu chức năng cho hệ thống Quản lý quán ăn - Gọi món bằng QR Code, với 2 user chính là nhân viên và khách hàng:

### Yêu cầu chức năng

#### Với Khách hàng
1. **Xem thực đơn**:
   - Cho phép khách hàng quét mã QR tại bàn để xem menu.
   - Hiển thị danh sách các món ăn, bao gồm tên, mô tả, giá và thời gian chờ ước tính.

2. **Gọi món**:
   - Cho phép khách hàng chọn và thêm các món ăn vào giỏ hàng.
   - Gửi đơn hàng đến bếp và thông báo cho nhân viên phục vụ.

3. **Theo dõi tình trạng đơn hàng**:
   - Cập nhật tình trạng đơn hàng (đang chuẩn bị, đang giao, hoàn thành) và hiển thị cho khách hàng.
   - Cho phép khách hàng theo dõi tình trạng đơn hàng của mình.
4. **Đăng nhập**:
   - Khách hàng quét QR trên bàn để đăng nhập gọi món.
  
#### Với Nhân viên
1. **Quản lý menu (Dish)**:
   - Cho phép quản lý (thêm, sửa, xóa) các mục menu, bao gồm tên món, mô tả, hình ảnh, giá.
   - Phân loại menu theo các danh mục (khai vị, món chính, tráng miệng, v.v.).

2. **Quản lý đơn hàng**:
   - Hiển thị danh sách các đơn hàng chưa hoàn thành.
   - Cho phép nhân viên cập nhật tình trạng đơn hàng.
   - Hiển thị thông tin về khách hàng, món ăn và thời gian đặt hàng.

3. **Thống kê và báo cáo**:
   - Tạo báo cáo về doanh thu, số lượng đơn hàng, số lượng bàn đang sử dụng, ...
4. **Đăng nhập**
   - Nhân viên hoặc chủ nhà hàng đăng nhập vào hệ thống.
5. **Quản lý nhân viên**:
   - Thêm sửa xoá nhân viên, thay đổi role
6. **Quản lý tài khoản**:
   - Thay đổi thông tin cá nhân

### Yêu cầu phi chức năng

1. **Trải nghiệm người dùng**:
  - Giao diện người dùng phải direct, dễ sử dụng.
  - Ứng dụng phải có phản hồi nhanh, không bị treo, lag.
  - Ứng dụng phải có thể chạy trên các thiết bị di động (smartphone, tablet) thông dụng.

2. **Tính bảo mật**:
  - Đảm bảo an toàn thông tin cho khách hàng, như mã QR, thông tin đơn hàng.
  - Phân quyền truy cập phù hợp cho nhân viên.

3. **Tính sẵn sàng**:
  - Ứng dụng phải hoạt động ổn định, đáp ứng yêu cầu 24/7.

4. **Tính mở rộng**:
  - Thiết kế hệ thống phải có tính mở rộng, dễ dàng bổ sung thêm tính năng mới trong tương lai.