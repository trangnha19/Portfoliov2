# Kế Hoạch Xây Dựng Portfolio Website - Nguyễn Thị Trang Nhã (LinkedIn Integration Spec)

## 1. Cấu Trúc Thư Mục Hệ Thống & Tài Nguyên Thực Tế (Relative Paths Only)
Mọi đường dẫn tài nguyên được cấu hình chính xác tuyệt đối theo sơ đồ quản lý tệp tin thực tế trong folder `portfolio/`:
- Tệp tin CV PDF gốc: `./CV_Nguyen Thi Trang Nha.pdf`
- Đường dẫn LinkedIn cá nhân: `https://www.linkedin.com/in/trang-nha-nguyen-thi/?trk=opento_nprofile_details`
- Sơ đồ dự án 1: Chatbot TravelAI (`./ai/`)
- Sơ đồ dự án 2: Nam An Bird's Nest ERP System (`./yen/`)
- Sơ đồ dự án 3: Wonder Wood ERP (`./go/`)
- Sơ đồ dự án 4: Yummy Food ERP (`./tauhu/`)
- Sơ đồ dự án 5: The SHEA Mobile App (`./theshea/`)

---

## 2. Tiêu Chuẩn Gắn Link LinkedIn Toàn Hệ Thống (LinkedIn Link Spec)
* **Tích hợp liên kết LinkedIn**: Tất cả các vị trí có chứa biểu tượng hoặc chữ LinkedIn trên trang web (ví dụ: Icon trên Header, khối Footer, hoặc phần thông tin liên hệ Contact) bắt buộc phải được triển khai bằng thẻ `<a>` trỏ trực tiếp đến URL cá nhân của bạn.
* **Cấu hình mở tab mới an toàn**: Bổ sung thuộc tính `target="_blank"` và `rel="noopener noreferrer"` cho thẻ liên kết này nhằm đảm bảo khi người dùng click vào, trang LinkedIn cá nhân sẽ mở ra ở một tab hoàn toàn mới, không làm đè lên trang Portfolio hiện tại.

---

## 3. Tiêu Chuẩn Giữ Nguyên Tiếng Anh Cho Hệ Thống Sub-Tabs (Technical Tabs Spec)
* **Sub-Tabs Cố định Tiếng Anh**: Toàn bộ hệ thống nhãn chữ điều hướng phụ bên trong màn hình xem tài liệu chi tiết dự án bắt buộc phải **giữ nguyên 100% bằng tiếng Anh** ở cả chế độ `EN` và `VI` để đảm bảo tính chuyên nghiệp của thuật ngữ kỹ thuật BA. Các nhãn bao gồm: `WORKFLOW`, `USE CASE`, `UC SPEC`, `SEQUENCE DIAGRAM`, `ACTIVITY DIAGRAM`, `ERD`, `DFD`, `FIGMA`.
* **Việt hóa các phần còn lại của Banner**: Khi chọn chế độ tiếng Việt `VI`, phần Breadcrumb prefix trên đỉnh đổi thành `PORTFOLIO / KINH NGHIỆM`, tiêu đề lớn đổi sang tiếng Việt và đoạn văn mô tả (Summary) chuyển sang tiếng Việt động chạy theo từ điển 100%.

---

## 4. Quy Tắc Gióng Hàng & Thẩm Mỹ Khối Giao Diện Landing Page
* **Trục gióng hàng Header**: Mọi phân đoạn nội dung lớn trên Landing Page sử dụng chung một cấu trúc container bọc ngoài (`max-w-7xl mx-auto px-6 md:px-12`) để gióng thẳng hàng lề trái tuyệt đối với chữ "TRANG NHA" trên Header.
* **Bộ đôi nút Hero**: Nút `Download CV` (Mở PDF ở tab mới bằng `target="_blank"`) và `About Me` xếp song song trên 1 hàng ngang. Họ tên chia làm 2 dòng: "Nguyễn Thị" và "Trang Nhã" bằng chữ tiếng Việt gốc UTF-8.
* **Lưới 6 Card kĩ năng (image_6e7127.png)**: Hiển thị dạng lưới 2 cột thông tin tĩnh, tuyệt đối không chứa nút tương tác "View Details →".

---

## 5. Bản Đồ Dữ Liệu Từ Điển Dịch Thuật Chuẩn Hóa (Bilingual Dictionary Spec)
*(Duy trì cấu trúc mảng từ điển đa ngôn ngữ động cho 5 dự án, hỗ trợ dịch thuật 100% tiêu đề, tóm tắt banner và 4 gạch đầu dòng sang tiếng Việt khi bật chế độ `VI`).*