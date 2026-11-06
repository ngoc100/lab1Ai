# PLAN.md – DỰ ÁN GAME STORE

## 1. Giới thiệu dự án

**Tên dự án:** Game Store

Game Store là website thương mại điện tử chuyên bán các phụ kiện và thiết bị dành cho game thủ như bàn phím gaming, chuột gaming, tai nghe, bàn di chuột, tay cầm chơi game và ghế gaming.

Website giúp khách hàng dễ dàng tìm kiếm, xem thông tin sản phẩm, thêm sản phẩm vào giỏ hàng và đặt hàng trực tuyến.

## 2. Mục tiêu dự án

- Xây dựng website bán phụ kiện gaming bằng Spring Boot.
- Tạo giao diện thân thiện, dễ sử dụng.
- Quản lý sản phẩm, danh mục và đơn hàng.
- Hỗ trợ khách hàng đăng ký, đăng nhập và mua hàng.
- Hỗ trợ quản trị viên quản lý hoạt động của website.

## 3. Công nghệ sử dụng

| Công nghệ | Mục đích |
|---|---|
| Java 17 | Ngôn ngữ lập trình chính |
| Spring Boot | Xây dựng ứng dụng web |
| Spring MVC | Xử lý yêu cầu và điều hướng |
| Spring Data JPA | Làm việc với cơ sở dữ liệu |
| MySQL | Lưu trữ dữ liệu |
| Thymeleaf | Hiển thị giao diện |
| HTML, CSS, JavaScript | Xây dựng giao diện website |
| Bootstrap | Hỗ trợ thiết kế giao diện |
| Maven | Quản lý thư viện và build dự án |
| Visual Studio Code | Môi trường lập trình |

## 4. Các chức năng chính

### 4.1. Chức năng dành cho khách hàng

- Xem danh sách sản phẩm.
- Tìm kiếm sản phẩm theo tên.
- Lọc sản phẩm theo danh mục.
- Xem chi tiết sản phẩm.
- Đăng ký tài khoản.
- Đăng nhập và đăng xuất.
- Thêm sản phẩm vào giỏ hàng.
- Cập nhật số lượng sản phẩm trong giỏ hàng.
- Xóa sản phẩm khỏi giỏ hàng.
- Đặt hàng.
- Xem lịch sử đơn hàng.

### 4.2. Chức năng dành cho quản trị viên

- Đăng nhập trang quản trị.
- Quản lý sản phẩm (thêm, sửa, xóa).
- Quản lý danh mục sản phẩm.
- Quản lý tài khoản người dùng.
- Quản lý đơn hàng.
- Cập nhật trạng thái đơn hàng.
- Xem thống kê cơ bản về sản phẩm và đơn hàng.

## 5. Thiết kế giao diện

Website dự kiến có các trang:

1. **Trang chủ:** Hiển thị sản phẩm nổi bật và danh mục.
2. **Trang sản phẩm:** Hiển thị toàn bộ sản phẩm.
3. **Trang chi tiết sản phẩm:** Hiển thị hình ảnh, giá và mô tả.
4. **Trang đăng nhập:** Cho phép người dùng đăng nhập.
5. **Trang đăng ký:** Cho phép tạo tài khoản.
6. **Trang giỏ hàng:** Hiển thị sản phẩm đã chọn.
7. **Trang thanh toán:** Xác nhận thông tin đặt hàng.
8. **Trang đơn hàng:** Hiển thị lịch sử mua hàng.
9. **Trang quản trị:** Quản lý sản phẩm, người dùng và đơn hàng.

## 6. Thiết kế cơ sở dữ liệu

Dự kiến sử dụng các bảng:

| Bảng | Chức năng |
|---|---|
| Users | Lưu thông tin người dùng |
| Categories | Lưu danh mục sản phẩm |
| Products | Lưu thông tin sản phẩm |
| Cart | Lưu giỏ hàng |
| Cart_Details | Lưu chi tiết giỏ hàng |
| Orders | Lưu thông tin đơn hàng |
| Order_Details | Lưu chi tiết đơn hàng |

## 7. Kiến trúc dự án

Dự án sử dụng mô hình MVC kết hợp Spring Boot.

- **Model:** Đại diện cho dữ liệu và các đối tượng trong hệ thống.
- **View:** Hiển thị giao diện website bằng Thymeleaf.
- **Controller:** Tiếp nhận và xử lý yêu cầu từ người dùng.
- **Repository:** Làm việc với cơ sở dữ liệu thông qua Spring Data JPA.
- **Service:** Xử lý các nghiệp vụ của hệ thống.

## 8. Kế hoạch thực hiện

### Giai đoạn 1: Khởi tạo dự án
- Tạo dự án Spring Boot bằng Spring Initializr.
- Mở dự án bằng Visual Studio Code.
- Cài đặt các thư viện cần thiết.
- Build dự án thành công.

### Giai đoạn 2: Xây dựng cơ sở dữ liệu
- Tạo cơ sở dữ liệu MySQL.
- Xây dựng các bảng.
- Thiết lập quan hệ giữa các bảng.

### Giai đoạn 3: Xây dựng chức năng
- Xây dựng chức năng đăng ký và đăng nhập.
- Xây dựng chức năng quản lý sản phẩm.
- Xây dựng chức năng giỏ hàng.
- Xây dựng chức năng đặt hàng.
- Xây dựng trang quản trị.

### Giai đoạn 4: Thiết kế giao diện
- Thiết kế trang chủ.
- Thiết kế trang sản phẩm.
- Thiết kế trang chi tiết sản phẩm.
- Thiết kế các trang đăng nhập, đăng ký và giỏ hàng.
- Thiết kế giao diện quản trị.

### Giai đoạn 5: Kiểm thử và hoàn thiện
- Kiểm tra các chức năng.
- Sửa lỗi phát sinh.
- Kiểm tra kết nối cơ sở dữ liệu.
- Hoàn thiện giao diện.
- Chuẩn bị báo cáo và sản phẩm cuối cùng.

## 9. Kết quả mong đợi

Sau khi hoàn thành, dự án sẽ có một website Game Store có thể hỗ trợ khách hàng tìm kiếm và mua phụ kiện gaming trực tuyến, đồng thời giúp quản trị viên quản lý sản phẩm, tài khoản và đơn hàng một cách thuận tiện.