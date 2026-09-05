# TGT Shop - Website Bán Hàng PC & Linh Kiện Máy Tính Cao Cấp

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Bootstrap 5](https://img.shields.io/badge/Bootstrap-5.x-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)](https://getbootstrap.com/)
[![Responsive](https://img.shields.io/badge/Design-Responsive-success?style=for-the-badge)](#tính-năng-nổi-bật)

> **Website thương mại điện tử chuyên cung cấp máy tính để bàn (PC Gaming, PC Đồ Họa, PC Văn Phòng), linh kiện phần cứng và thiết bị ngoại vi với giao diện hiện đại, tối ưu trải nghiệm người dùng trên mọi kích cỡ màn hình.**

---

## Tổng quan dự án

TGT Shop là một ứng dụng web bán hàng hoàn chỉnh mô phỏng các nghiệp vụ thương mại điện tử thực tế. Website được xây dựng với cấu trúc mã nguồn tối ưu bằng HTML5, CSS3, JavaScript ES6 và Bootstrap, cung cấp đầy đủ chu trình mua sắm từ tìm kiếm, xem chi tiết, giỏ hàng, thanh toán đa phương thức đến in hóa đơn xác nhận.

Hệ thống quản lý trạng thái phiên đăng nhập và dữ liệu đơn hàng phía Client thông qua `localStorage`, đảm bảo dữ liệu mua sắm được bảo lưu xuyên suốt quá trình tương tác mà không bị mất đi khi làm mới trang.

---

## Tính năng nổi bật

### 1. Trang chủ & Giới thiệu sản phẩm
- Banner quảng cáo và thanh trượt (Carousel) trình diễn các bộ máy PC nổi bật và chương trình khuyến mãi theo mùa.
- Phân loại trực quan các danh mục sản phẩm thịnh hành: PC Gaming, PC Workstation, Linh kiện phần cứng, Màn hình, Bàn phím cơ.

### 2. Danh mục sản phẩm & Bộ lọc thông minh
- Hiển thị danh sách sản phẩm với thẻ thông tin chi tiết: tên linh kiện, cấu hình vắn tắt, giá niêm yết và trạng thái còn hàng.
- Tìm kiếm tức thì theo tên hoặc từ khóa sản phẩm.
- Bộ lọc nâng cao theo khoảng giá, danh mục và thương hiệu.
- Sắp xếp linh hoạt: giá tăng dần, giá giảm dần, bảng chữ cái A-Z và Z-A.

### 3. Trang chi tiết sản phẩm
- Thư viện ảnh sản phẩm độ nét cao với tính năng chuyển đổi ảnh đại diện.
- Bảng thông số kỹ thuật chi tiết (CPU, GPU, RAM, Mainboard, PSU, Tản nhiệt, Bảo hành).
- Điều chỉnh số lượng và thêm trực tiếp vào giỏ hàng.

### 4. Quản lý Giỏ hàng (Shopping Cart)
- Thêm, giảm số lượng hoặc loại bỏ sản phẩm nhanh chóng.
- Tự động tính toán tổng tiền hàng, tiền thuế và phí giao hàng theo thời gian thực.
- Đồng bộ hóa dữ liệu giỏ hàng vào `localStorage` của trình duyệt.

### 5. Quy trình Đặt hàng & Thanh toán (Checkout Workflow)
- Thu thập thông tin giao hàng: Họ tên, số điện thoại, địa chỉ nhận hàng, ghi chú đơn hàng.
- Lựa chọn linh hoạt các hình thức thanh toán phổ biến:
  - Thanh toán khi nhận hàng (COD).
  - Chuyển khoản ngân hàng trực tuyến.
  - Thanh toán qua ví điện tử MoMo.
- Cơ chế xác thực mã CAPTCHA trước khi hoàn tất giao dịch nhằm ngăn chặn hành vi spam đơn hàng tự động.

### 6. Xuất & In Hóa đơn mua hàng (Invoice)
- Hiển thị tóm tắt toàn bộ thông tin đơn hàng sau khi giao dịch thành công.
- Hỗ trợ nút in hóa đơn trực tiếp từ trình duyệt phục vụ lưu trữ hoặc bảo hành.

### 7. Xác thực & Quản lý người dùng
- Đăng ký tài khoản mới kèm bước nhập mã kích hoạt bảo mật.
- Đăng nhập, ghi nhớ phiên làm việc và hiển thị tên người dùng trên thanh điều hướng.
- Tự động dọn dẹp và bảo toàn giỏ hàng tương ứng khi người dùng chuyển đổi trạng thái đăng nhập/đăng xuất.

---

## Cấu trúc thư mục dự án

```
CuaHangMayTinh-TGTShop/
├── html/
│   ├── index.html                  # Trang chủ giới thiệu
│   ├── products.html               # Trang danh sách & bộ lọc sản phẩm
│   ├── product-detail.html         # Trang chi tiết thông số sản phẩm
│   ├── cart.html                   # Trang giỏ hàng
│   ├── checkout.html               # Trang nhập thông tin thanh toán
│   ├── verification_payment.html   # Trang xác thực CAPTCHA thanh toán
│   ├── invoice.html                # Trang hóa đơn mua hàng hoàn tất
│   ├── register.html               # Trang đăng ký thành viên
│   ├── login.html                  # Trang đăng nhập
│   └── verification.html           # Trang kích hoạt tài khoản
├── css/                            # Các file stylesheet định kiểu giao diện
├── js/
│   ├── main.js                     # Xử lý logic nghiệp vụ, giỏ hàng & localStorage
│   └── bootstrap.min.js            # Thư viện JavaScript hỗ trợ giao diện Bootstrap
├── img/                            # Hình ảnh sản phẩm, banner và logo thương hiệu
└── README.md                       # Tài liệu hướng dẫn dự án
```

---

## Công nghệ & Kỹ thuật áp dụng

| Thành phần | Công nghệ | Ứng dụng cụ thể |
|---|---|---|
| **Cấu trúc web** | HTML5 Semantic Tags | Sử dụng các thẻ ngữ nghĩa (`header`, `nav`, `section`, `article`, `footer`) chuẩn SEO |
| **Định dạng giao diện** | CSS3 & Flexbox / Grid | Tùy biến kiểu dáng màu sắc hiện đại, hiệu ứng hover mượt mà |
| **Responsive Design** | Bootstrap 5 | Đảm bảo trang web hiển thị tối ưu trên Desktop, Tablet và Smartphone |
| **Logic & Tương tác** | JavaScript (ES6+) | Thao tác DOM, xử lý sự kiện, tính toán giỏ hàng, xác thực form |
| **Client Storage** | HTML5 LocalStorage | Lưu trữ dữ liệu giỏ hàng, thông tin tài khoản và lịch sử đặt hàng phía trình duyệt |

---

## Hướng dẫn cài đặt & Chạy dự án

Website hoạt động hoàn toàn ở phía máy khách (Front-end Static Web), không cần cài đặt môi trường máy chủ phức tạp:

### Cách 1: Chạy trực tiếp từ trình duyệt
1. Clone repository về máy tính:
   ```bash
   git clone https://github.com/snizyboi0165/CuaHangMayTinh-TGTShop.git
   ```
2. Truy cập vào thư mục `CuaHangMayTinh-TGTShop/html/`.
3. Nhấp đúp chuột vào file `index.html` để mở trang web bằng trình duyệt bất kỳ (Chrome, Edge, Firefox, Brave).

### Cách 2: Sử dụng Live Server trong VS Code (Khuyến nghị)
1. Mở thư mục dự án trong **Visual Studio Code**.
2. Cài đặt tiện ích mở rộng **Live Server** (của tác giả Ritwick Dey).
3. Nhấp chuột phải vào file `html/index.html` và chọn **Open with Live Server**.
4. Website sẽ tự động khởi chạy tại địa chỉ `http://127.0.0.1:5500/html/index.html`.
