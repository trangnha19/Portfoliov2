/plan
Tôi muốn xây dựng một website portfolio cá nhân mini với các yêu cầu sau:

1. **Cấu trúc kỹ thuật**: 
   - Sử dụng HTML5, Tailwind CSS (qua CDN) và React JS (qua Babel/CDN để có thể chạy trực tiếp trên trình duyệt mà không cần build step).
   - Mục tiêu: Khi mở trực tiếp file `index.html` từ thư mục, website phải hoạt động đầy đủ các tính năng (chuyển tab, load nội dung).

2. **Yêu cầu về đường dẫn**:
   - Tất cả các asset (JS, CSS nội bộ nếu có, hình ảnh, video) phải sử dụng **đường dẫn tương đối (relative paths)**. 
   - Đảm bảo khi copy cả folder `portfolio` sang máy tính khác, trang web vẫn hiển thị đúng.

3. **Giao diện & Chức năng**:
   - Dựa trên hình ảnh `index.png` có sẵn trong thư mục để thiết kế layout.
   - Các tab nội dung (ví dụ: Giới thiệu, Dự án, Liên hệ) phải có hiệu ứng chuyển đổi mượt mà bằng React state.
   - Sử dụng Lucide Icons (CDN) để đồng bộ với phong cách thiết kế chuyên nghiệp.

4. **Nhiệm vụ của bạn**:
   - Phân tích hình ảnh `index.png` để bóc tách các component (Header, Sidebar, Main Content, v.v.).
   - Lên kế hoạch chi tiết về cấu trúc thư mục và cách tổ chức code trong file `index.html`.
   - **XUẤT KẾT QUẢ**: Hãy lưu toàn bộ kế hoạch này vào một file tên là `plan.md` trong thư mục hiện tại. Không thực thi viết code ngay lúc này.

Hãy bắt đầu phân tích `index.png` và lập kế hoạch vào `plan.md`.
--------

Dựa trên file `plan.md` và hình ảnh `index.png` có trong thư mục, hãy triển khai mã nguồn hoàn chỉnh cho file `index.html`. 

**Các yêu cầu nghiêm ngặt cần tuân thủ:**
1. **Kiến trúc Single-file:** Tất cả code HTML, CSS tùy chỉnh và React (JSX) phải nằm trọn trong một file `index.html` duy nhất.
2. **Thiết lập CDN:** Sử dụng đúng các link CDN đã liệt kê trong plan (React 18, Babel, Tailwind, Lucide React) để đảm bảo file chạy được ngay khi mở trực tiếp bằng trình duyệt (giao thức file://).
3. **Đường dẫn tương đối:** Tuyệt đối sử dụng relative paths (ví dụ: `./assets/images/index.png`) cho toàn bộ tài nguyên. Đảm bảo tính "portable" để khi copy folder đi nơi khác web vẫn hoạt động.
4. **Đồng bộ Layout:** Kết hợp bố cục "Sidebar + Main Content" từ plan.md và chi tiết thiết kế từ hình ảnh `index.png`. Hãy chú trọng vào các hiệu ứng transition khi chuyển tab và animation cho thanh Skill bar.
5. **Dữ liệu:** Sử dụng phần dữ liệu mẫu trong mục 8 của `plan.md` để đổ vào các component, nhưng hãy tối ưu hóa nội dung để trông chuyên nghiệp nhất.

Bây giờ, hãy tạo file `index.html` và viết code hoàn chỉnh.
---------
Hãy đọc kỹ file `plan.md` và thực hiện triển khai mã nguồn cho website portfolio này.

**Yêu cầu kỹ thuật chi tiết:**
1. **Cấu trúc file**: Tạo một file duy nhất là `index.html`. Toàn bộ logic React (JSX), CSS tùy chỉnh và HTML phải nằm trong file này.
2. **Thiết lập môi trường**: 
   - Sử dụng các link CDN cho React 18, Babel standalone, Tailwind CSS và Lucide Icons như đã liệt kê trong plan.
   - Đảm bảo file có thể chạy trực tiếp bằng cách mở trong trình duyệt (giao thức `file://`) mà không cần máy chủ local.
3. **Quản lý Assets**: 
   - Sử dụng đường dẫn tương đối (Relative paths) chính xác: `./screenshots/ava.png`, `./screenshots/cv1.jpg`, và `./screenshots/cv2.png`.
   - Thiết kế tab "CV Viewer" để hiển thị hai ảnh CV trang 1 và trang 2 theo chiều dọc, tối ưu để người xem có thể đọc nội dung CV dễ dàng.
4. **Giao diện & Trải nghiệm (UI/UX)**:
   - Sử dụng hệ màu Xanh Navy (#1e3a8a) và Vàng Gold (#d4af37) để tạo cảm giác chuyên nghiệp cho vị trí Business Analyst.
   - Triển khai React `useState` để chuyển đổi giữa các tab: About, Experience, Projects, Skills, và CV.
   - Các thẻ dự án (TravelAI, Yến Sào Nam An ERP,...) cần có icon Lucide tương ứng và hiệu ứng hover tinh tế.
5. **Nội dung**: Sử dụng chính xác các thông tin về học vấn (GPA 3.72), chứng chỉ (IELTS 6.5, HSK 3) và kinh nghiệm làm việc từ file `plan.md`.

Hãy viết code hoàn chỉnh và tối ưu nhất cho tôi.

---
Hãy đọc kỹ file `plan.md` và phân tích các hình ảnh giao diện trong thư mục `screenshots/` (đặc biệt là `main.png` và `ai1.png`) để triển khai mã nguồn hoàn chỉnh cho trang web portfolio này.

**Các yêu cầu kỹ thuật bắt buộc khi code:**
1. **Single-file Architecture**: Toàn bộ mã nguồn bao gồm HTML5, logic React JS (JSX), và các đoạn cấu hình Tailwind CSS custom theme phải nằm gọn trong duy nhất một file `index.html`[cite: 3].
2. **Cấu hình Hệ màu & Font**: Khai báo chính xác cấu hình `tailwind.config` trong file với các mã màu (`baDark`, `baGold`, `baBgLight`, `baTextMuted`) và phong cách chữ Serif/Sans-serif như đặc tả trong mục 3 của plan[cite: 3].
3. **Quản lý SPA Tabs**: Sử dụng React `useState` để bắt sự kiện click trên thanh Navbar (`HOME`, `ABOUT`, `SKILLS`, `EXPERIENCE`, `CONTACT`, `CV VIEWER`) nhằm chuyển đổi mượt mà giữa các vùng nội dung mà không bị load lại trang[cite: 3].
4. **Đường dẫn tương đối (Relative paths)**: Đảm bảo sử dụng chính xác các đường dẫn `./screenshots/ava.png`, `./screenshots/cv1.jpg`, `./screenshots/cv2.png`, và `./screenshots/ai1.png` để đồ án chạy offline tốt khi mở trực tiếp file bằng trình duyệt (giao thức file://)[cite: 3].
5. **Đổ dữ liệu thực tế**: Điền đầy đủ, chính xác các thông tin cá nhân (GPA 3.72), bộ kỹ năng, và chuỗi 5 dự án lớn (TravelAI, Yến Sào Nam An ERP,...) từ mục 4 và mục 5 trong plan vào giao diện[cite: 3].
6. **Cách gọi Lucide Icons**: Vì sử dụng qua CDN, hãy import và gọi icon theo cú pháp global (ví dụ: `const { Mail, Phone, Linkedin, Download, ArrowRight } = window.lucide;`) để tránh lỗi render[cite: 3].

Hãy tiến hành viết mã nguồn hoàn chỉnh cho file `index.html` ngay bây giờ.
---
Hãy đọc kỹ file `plan.md` và phân tích toàn bộ chuỗi hình ảnh giao diện trong thư mục `screenshots/` (đặc biệt là bố cục toàn trang `main.png` và ảnh dự án `ai1.png`) để triển khai mã nguồn cho website portfolio này.

**Các yêu cầu kỹ thuật và trải nghiệm người dùng bắt buộc:**
1. **Single-file Architecture**: Toàn bộ mã nguồn bao gồm HTML5, logic React JS (JSX), và cấu hình Tailwind CSS custom theme phải nằm trọn vẹn trong duy nhất một file `index.html`.
2. **Cơ chế Tương tác Cuộn (Smooth Scroll)**: 
   - Website hoạt động theo dạng One-Page Landing Page dài. Phân chia các phân đoạn nội dung bằng thẻ ID rõ rệt: `id="home"`, `id="about"`, `id="skills"`, `id="experience"`, `id="contact"`.
   - Khi click vào các nút tương ứng trên thanh Navbar cố định (Sticky Header), sử dụng React hoặc thuộc tính CSS để kích hoạt hiệu ứng lướt cuộn mượt mà (Smooth Scroll) xuống đúng phân đoạn đó, không dùng cơ chế chuyển tab ẩn/hiện nội dung.
3. **Cấu hình Hệ màu & Font**: Khai báo chính xác cấu hình `tailwind.config` khớp với mã màu Figma trong mục 3 của plan (Xanh Navy đậm `baDark`, Vàng Gold `baGold`, Nền `baBgLight`). Sử dụng font Serif sang trọng cho các tiêu đề lớn đúng như hình ảnh thiết kế.
4. **Đường dẫn tương đối (Relative paths)**: Đảm bảo sử dụng chính xác các đường dẫn tài nguyên: `./screenshots/ava.png` và `./screenshots/ai1.png`. Website phải vận hành offline hoàn hảo khi mở trực tiếp file bằng trình duyệt (giao thức file://).
5. **Đổ dữ liệu & Giao diện**: 
   - Tuyệt đối không tích hợp phần CV Viewer hay hiển thị ảnh `cv1.jpg`/`cv2.png` trên trang. Nút "Download CV" sẽ là một liên kết (link) tải file thông thường.
   - Điền đầy đủ dữ liệu thực tế: Thông tin cá nhân (GPA 3.72), bộ 4 thẻ Skills, và timeline 5 dự án lớn (TravelAI có kèm ảnh minh họa `ai1.png`, Yến Sào Nam An ERP,...) vào đúng cấu trúc giao diện.
6. **Cách gọi Lucide Icons**: Vì nhúng qua CDN, hãy import và gọi icon theo cú pháp global từ thư viện toàn cục (ví dụ: `const { Mail, Phone, Linkedin, Download, ArrowRight } = window.lucide;`) để tránh lỗi render.

Hãy tiến hành viết mã nguồn hoàn chỉnh cho file `index.html` ngay bây giờ.
----
Hãy đọc kỹ file `plan.md` vừa được hiệu chỉnh và đối chiếu trực quan với chuỗi hình ảnh thiết kế từ `main1.jpeg` đến `main7.jpeg` trong thư mục `screenshots/` để viết lại toàn bộ mã nguồn cho file `index.html`.

**Các nguyên tắc lập trình bắt buộc để đạt tỷ lệ giống Figma cao nhất:**
1. **Single-file Codebase**: Gói gọn toàn bộ cấu trúc HTML5, các đoạn mã cấu hình hệ màu custom theme của Tailwind, và logic điều hướng của React JS trong duy nhất file `index.html`.
2. **Cấu chế One-Page Smooth Scroll**: 
   - Không thiết kế ẩn/hiện tab. Toàn bộ nội dung trang phải được hiển thị tuần tự từ trên xuống dưới theo chiều dọc.
   - Gắn chính xác các thuộc tính ID (`id="home"`, `id="about"`, `id="skills"`, `id="experience"`, `id="contact"`) vào các thẻ section tương ứng. 
   - Khi bấm vào các nút menu trên Navbar cố định (Sticky Header), trang phải lướt cuộn mượt mà (Smooth Scroll) đến đúng phân đoạn đó. Sử dụng thuộc tính `scroll-mt-20` của Tailwind để không bị thanh Header che mất tiêu đề các phần.
3. **Độ chính xác về Màu sắc và Typography**:
   - Sử dụng đúng mã màu được trích xuất từ thiết kế: Xanh Navy đậm (`#1a2b49`), Vàng đất/Gold nhạt (`#c2a67f`), Nền xám trắng nhạt (`#fbfbfb`).
   - Nhúng link Google Fonts cho font chữ Serif (Playfair Display) để áp dụng cho tất cả các tiêu đề lớn: "Nguyễn Thị Trang Nhã", "Who I Am", "My Skills", "Work Journey", "Let's Connect".
4. **Loại bỏ CV Viewer**: Tuyệt đối không tích hợp vùng hiển thị ảnh CV (`cv1.jpg`, `cv2.png`) trên trang. Nút "Download CV" ở khối Hero sẽ hoạt động như một thẻ liên kết tải file thông thường.
5. **Giao diện Khối Hero & Thẻ**: Tái hiện đúng khối vát chéo màu xanh sẫm bên trái trang chủ, khung ảnh đại diện Polaroid màu trắng có bóng đổ mềm, nhãn "Available for work" ghim ở góc, lưới 2 cột cho phần Skills, và trục timeline chỉ dọc màu vàng Gold cho phần Experience.
6. **Import Icon Lucide**: Khai báo bóc tách icon toàn cục (ví dụ: `const { Mail, Phone, Linkedin, Download, ArrowRight, Monitor, Figma, FileText, Users } = window.lucide;`) ở đầu thẻ script React để đảm bảo hiển thị đúng các biểu tượng icon trên các card.

Hãy viết lại mã nguồn file `index.html` hoàn chỉnh, sạch đẹp và giống Figma nhất cho tôi ngay bây giờ.
----
Tôi đã gửi kèm hai bức ảnh đối chiếu: ảnh bên trái là giao diện hiện tại bạn vừa code bị lỗi, ảnh bên phải là giao diện gốc chuẩn từ Figma mà tôi muốn đạt được. Đồng thời tôi đã cập nhật file `plan.md` chi tiết. 

Hãy sửa lại toàn bộ file `index.html` để đạt độ chính xác Pixel-Perfect so với ảnh bên phải:

1. **Sửa đổi ảnh đại diện (Avatar Source)**: Đổi nguồn file ảnh từ `ava.png` sang chính xác `./screenshots/ava1.png`.
2. **Sửa góc vát chéo của khối Hero (Clip-path)**: Khối màu xanh `figmaDark` bên trái hiện tại đang bị vát chéo sai góc. Hãy sửa lại phần CSS `clip-path: polygon(...)` sao cho cạnh chéo đi từ góc trên bên phải hướng thu hẹp dần xuống phía dưới (góc trên nhọn rộng, góc dưới hẹp lại) giống hệt ảnh Figma mẫu.
3. **Sửa nút bấm "About Me"**: Sửa từ nút dạng viền trong suốt sang dạng nút có nền trắng tinh (`bg-white`), chữ màu đen/xanh sẫm, bo góc và có icon mũi tên `→` chỉ sang phải rõ ràng.
4. **Căn chỉnh khung ảnh Polaroid bên phải**:
   - Khung viền ảnh phải là màu trắng tinh, bo góc nhẹ, đổ bóng rất mềm diện rộng (`shadow-2xl`).
   - Áp dụng hiệu ứng xoay nghiêng nhẹ (khoảng `rotate-2` hoặc `-rotate-1` tùy chỉnh tùy góc độ) để tạo độ nghiêng tự nhiên nghệ thuật y hệt ảnh mẫu.
   - Định vị chính xác nhãn `Available for work` nằm đè lên viền trên khối ảnh, và nhãn `IELTS 6.5 - HSK3` đè lên viền dưới khối ảnh.
5. **Cơ chế trang**: Giữ nguyên cấu trúc One-Page Smooth Scroll theo các ID đã định nghĩa trong plan.md. Không tích hợp phần CV Viewer.

Hãy đọc kỹ hình ảnh đối chiếu và file `plan.md` để xuất ra file `index.html` hoàn mỹ nhất.
--
Tôi vừa cập nhật lại file `plan.md` để bổ sung đặc tả màu chữ cho tiêu đề khối Hero theo bức ảnh cận cảnh mới gửi. Hãy viết lại toàn bộ mã nguồn `index.html` đáp ứng tiêu chí sau:

1. **Phối màu chữ tiêu đề Tên chính xác**:
   - Tiêu đề lớn sử dụng font Serif (Playfair Display) được chia làm 2 dòng.
   - Dòng trên chữ "Nguyễn Thị" sử dụng mã màu vàng đất của figma (`text-figmaGold`).
   - Dòng dưới chữ "Trang Nhã" bắt buộc phải sử dụng màu trắng tinh (`text-white`).
2. **Sửa đổi ảnh đại diện (Avatar Source)**: Sử dụng chính xác file `./screenshots/ava1.png`.
3. **Sửa góc vát chéo của khối Hero (Clip-path)**: Đảm bảo khối màu xanh `figmaDark` bên trái vát chéo sắc nét với phần trên rộng, phần dưới hẹp lại theo đúng thiết kế gốc chuẩn `main1.jpeg`.
4. **Sửa nút bấm "About Me"**: Nút có nền trắng tinh (`bg-white`), chữ đen, bo góc nhẹ và có icon mũi tên `→`.
5. **Khung ảnh Polaroid bên phải**: Nền trắng, bo góc nhẹ, đổ bóng mềm rộng (`shadow-2xl`), và xoay nghiêng nhẹ góc (`rotate-2`) tự nhiên. Căn vị trí 2 nhãn "Available for work" và "IELTS 6.5 - HSK3" chuẩn chỉnh đè lên viền khung ảnh.
6. **Cơ chế hoạt động**: One-Page Landing Page lướt cuộn mượt mà (Smooth Scroll) qua các ID phần nội dung. Không chứa phần hiển thị CV Viewer.

Hãy thực thi viết lại code file `index.html` hoàn mỹ nhất.
---
Hãy đọc kỹ file `plan.md` vừa được cập nhật cấu trúc và phân tích chi tiết sơ đồ danh sách tệp tin thực tế trong thư mục `ai/` (như workflow.png, usecase1.png, ucspe1.png, se1.png, erd.png, fig1.png) để lập trình hoàn chỉnh file `index.html`.

**Các yêu cầu kỹ thuật liên kết hình ảnh động:**
1. **Quản lý Màn hình Xem chi tiết (Selected Project)**:
   - Cấu hình React State `const [selectedProject, setSelectedProject] = useState(null);`. Khi click nút `View Details →` của TravelAI, kích hoạt màn hình tài liệu đặc tả hệ thống.
   - Thiết kế nút `← Back` ở góc trên cùng bên trái màn hình chi tiết để quay lại giao diện Landing Page chính.
2. **Xây dựng Thanh Sub-Tabs Tài Liệu Gốc**:
   - Tạo hệ thống menu gồm 6 tab tài liệu phụ: `WORKFLOW`, `USE CASE`, `UC SPEC`, `SEQUENCE DIAGRAM`, `ERD`, `FIGMA`. 
   - Quản lý việc hoán đổi bằng React State để load động các file ảnh sơ đồ thực tế nằm trực tiếp trong thư mục `./ai/` theo đúng logic đường dẫn tương đối sau:
     * Tab WORKFLOW: Hiển thị `./ai/workflow.png`
     * Tab USE CASE: Hiển thị `./ai/usecase1.png`
     * Tab UC SPEC: Hiển thị xếp chồng theo chiều dọc (Vertical Stack) 2 file `./ai/ucspe1.png` và `./ai/ucspe2.png`
     * Tab SEQUENCE DIAGRAM: Hiển thị xếp chồng theo chiều dọc chuỗi file từ `./ai/se1.png` đến `./ai/se4.png`
     * Tab ERD: Hiển thị `./ai/erd.png`
     * Tab FIGMA: Hiển thị xếp chồng chuỗi ảnh giao diện từ `./ai/fig1.png` đến `./ai/fig7.png`
   - Tất cả các ảnh sơ đồ hiển thị phải căn giữa trang, bao bọc trong khung thẻ div nền trắng, có bo góc và bóng đổ nhẹ, giữ nguyên độ nét để đọc được văn bản.
3. **Độ chính xác UI/UX Màn hình chính**:
   - Tiêu đề khối Hero có dòng 1 "Nguyễn Thị" màu vàng gold (`text-figmaGold`) và dòng 2 "Trang Nhã" màu trắng tinh (`text-white`) trên nền khối vát chéo xanh Navy sẫm.
   - Khung ảnh đại diện Polaroid chứa ảnh `./screenshots/ava1.png` có độ xoay nghiêng nhẹ kèm nhãn ghim trạng thái. Menu chính hoạt động theo cơ chế One-Page Smooth Scroll bằng ID.

Hãy thực thi viết toàn bộ mã nguồn hoàn chỉnh vào file `index.html` ngay bây giờ.
----
Hãy đọc kỹ file `plan.md` vừa được cập nhật cấu trúc và phân tích chi tiết chuỗi hình ảnh tài liệu đặc tả trong thư mục con `screenshots/projects/ai/` (từ `ai1.png` đến `ai6.jpg`) để lập trình hoàn chỉnh file `index.html`.

**Các yêu cầu kỹ thuật xử lý thư mục và load ảnh động:**
1. **Quản lý Màn hình Xem chi tiết (Selected Project)**:
   - Cấu hình React State `const [selectedProject, setSelectedProject] = useState(null);`. Khi click nút `View Details →` của TravelAI, kích hoạt màn hình tài liệu đặc tả hệ thống.
   - Thiết kế nút `← Back` ở góc trên cùng bên trái màn hình chi tiết, cho phép gọi hàm `setSelectedProject(null)` để quay lại giao diện Landing Page chính.
2. **Xây dựng Thanh Sub-Tabs Phụ đổi ảnh động**:
   - Tạo hệ thống menu gồm 6 tab: `WORKFLOW`, `USE CASE`, `UC SPEC`, `SEQUENCE DIAGRAM`, `ERD`, `FIGMA`. 
   - Quản lý việc chuyển đổi bằng React State để load động các file ảnh sơ đồ thực tế nằm trong thư mục con `ai/` theo đúng đường dẫn tương đối sau:
     * Tab WORKFLOW: `./screenshots/projects/ai/ai1.png`
     * Tab USE CASE: `./screenshots/projects/ai/ai2.jpg`
     * Tab UC SPEC: `./screenshots/projects/ai/ai3.jpg`
     * Tab SEQUENCE DIAGRAM: `./screenshots/projects/ai/ai4.png`
     * Tab ERD: `./screenshots/projects/ai/ai5.jpg`
     * Tab FIGMA: `./screenshots/projects/ai/ai6.jpg`
   - Đảm bảo ảnh hiển thị rõ ràng, căn giữa trang, bao bọc trong khung thẻ div nền trắng có bo góc và bóng đổ nhẹ y hệt ảnh mẫu.
3. **Độ chính xác UI/UX Màn hình chính**:
   - Đảm bảo tiêu đề khối Hero có dòng 1 "Nguyễn Thị" màu vàng gold (`text-figmaGold`) và dòng 2 "Trang Nhã" màu trắng tinh (`text-white`) trên nền khối vát chéo xanh Navy sẫm.
   - Khung ảnh đại diện Polaroid chứa ảnh đại diện `./screenshots/ava1.png` có độ xoay nghiêng nhẹ tự nhiên kèm 2 nhãn trạng thái ghim trên khung.
   - Menu chính hoạt động theo cơ chế One-Page Smooth Scroll bằng ID, không chứa phần hiển thị ảnh CV Viewer cũ.

Hãy tiến hành viết toàn bộ mã nguồn hoàn chỉnh vào file `index.html`.
----
Hãy đọc kỹ file `plan.md` vừa được nâng cấp cấu trúc và phân tích kỹ bức ảnh minh họa bố cục `ai2.jpg` để lập trình cơ chế xếp chồng sơ đồ theo chiều dọc cho file `index.html`.

**Các chỉ thị logic quan trọng cho phần View Details:**
1. **Cơ chế Xếp chồng Ảnh theo chiều dọc (Vertical Stack Layout)**:
   - Trong màn hình chi tiết dự án TravelAI, khi người dùng tương tác với thanh Sub-Tabs phụ, hãy thiết kế vùng hiển thị nội dung là một danh sách ảnh cuộn dọc (`flex flex-col space-y-12 items-center`) dựa trên các mảng dữ liệu đường dẫn tương đối sau:
     * Chọn tab **WORKFLOW**: Hiển thị 1 ảnh `./ai/workflow.png`.
     * Chọn tab **USE CASE**: Hiển thị nối tiếp nhau 3 ảnh: `./ai/usecase1.png` (có tiêu đề phụ "OVERALL USE CASE DIAGRAM"), `./ai/usecase2.png` (tiêu đề "LEVEL 1 USE CASE DIAGRAM"), và `./ai/usecase3.png` (tiêu đề "LEVEL 2 USE CASE DIAGRAM") y hệt như bố cục sắp xếp của ảnh minh họa figma gốc `ai2.jpg`.
     * Chọn tab **UC SPEC**: Hiển thị nối tiếp nhau 2 ảnh `./ai/ucspe1.png` và `./ai/ucspe2.png`.
     * Chọn tab **SEQUENCE DIAGRAM**: Hiển thị nối tiếp chuỗi 4 ảnh từ `./ai/se1.png` đến `./ai/se4.png`.
     * Chọn tab **ERD**: Hiển thị 1 ảnh `./ai/erd.png`.
     * Chọn tab **FIGMA**: Hiển thị nối tiếp chuỗi ảnh giao diện từ `./ai/fig1.png` đến `./ai/fig3.png`.
   - Đảm bảo tất cả các hình ảnh sơ đồ hiển thị đều giữ nguyên tỷ lệ, độ rộng hợp lý (`w-full max-w-5xl h-auto`), hiển thị sắc nét, rõ chữ.
2. **Độ chính xác UI/UX Màn hình chính**:
   - Thiết kế nút `← Back` ở góc trên bên trái để quay lại giao diện Landing Page (sử dụng hàm đặt trạng thái `selectedProject` về null).
   - Tiêu đề khối Hero có dòng 1 "Nguyễn Thị" màu vàng gold (`text-figmaGold`) và dòng 2 "Trang Nhã" màu trắng tinh (`text-white`) trên nền khối vát chéo xanh Navy sẫm. Khung ảnh Polaroid chứa ảnh `./screenshots/ava1.png` có độ xoay nghiêng nhẹ tự nhiên.

Hãy thực thi viết toàn bộ mã nguồn hoàn chỉnh vào file `index.html` ngay bây giờ.
----
Hãy đọc kỹ file `plan.md` vừa được cập nhật và phân tích chuỗi ảnh bố cục phân tầng `image_190a48.png`, `image_190a64.png`, `image_190a6a.png` để lập trình cơ chế xếp chồng sơ đồ theo chiều dọc cho file `index.html`.

**Các chỉ thị logic quan trọng cho phần View Details:**
1. **Cơ chế Xếp chồng Ảnh theo chiều dọc (Vertical Stack Layout)**:
   - Trong màn hình chi tiết dự án TravelAI, khi người dùng tương tác với thanh Sub-Tabs phụ, hãy thiết kế vùng hiển thị nội dung là một danh sách ảnh cuộn dọc (`flex flex-col space-y-12 items-start w-full`) dựa trên các mảng dữ liệu đường dẫn tương đối sau:
     * Chọn tab **WORKFLOW**: Hiển thị 1 ảnh `./ai/workflow.png`.
     * Chọn tab **USE CASE**: Hiển thị nối tiếp nhau 3 khối nội dung: Khối 1 có tiêu đề phụ "| OVERALL USE CASE DIAGRAM" (màu font `text-figmaGold` font-serif) đi kèm ảnh `./ai/usecase1.png`. Khối 2 có tiêu đề phụ "| LEVEL 1 USE CASE DIAGRAM" đi kèm ảnh `./ai/usecase2.png`. Khối 3 có tiêu đề phụ "| LEVEL 2 USE CASE DIAGRAM" đi kèm ảnh `./ai/usecase3.png`. Cấu trúc sắp xếp này phải chính xác theo luồng phân rã tài liệu BA của ảnh minh họa `image_190a64.png` và `image_190a6a.png`.
     * Chọn tab **UC SPEC**: Hiển thị nối tiếp nhau 2 ảnh `./ai/ucspe1.png` và `./ai/ucspe2.png`.
     * Chọn tab **SEQUENCE DIAGRAM**: Hiển thị nối tiếp chuỗi 4 ảnh từ `./ai/se1.png` đến `./ai/se4.png`.
     * Chọn tab **ERD**: Hiển thị 1 ảnh `./ai/erd.png`.
     * Chọn tab **FIGMA**: Hiển thị nối tiếp chuỗi ảnh giao diện từ `./ai/fig1.png` đến `./ai/fig3.png`.
   - Đảm bảo tất cả các hình ảnh sơ đồ hiển thị đều giữ nguyên tỷ lệ, độ rộng lớn dễ đọc (`w-full max-w-5xl mx-auto h-auto shadow-sm border rounded-lg bg-white p-4`), hiển thị sắc nét, rõ chữ.
2. **Độ chính xác UI/UX Màn hình chính**:
   - Thiết kế nút `← Back` ở góc trên bên trái để quay lại giao diện Landing Page (sử dụng hàm đặt trạng thái `selectedProject` về null).
   - Tiêu đề khối Hero có dòng 1 "Nguyễn Thị" màu vàng gold (`text-figmaGold`) và dòng 2 "Trang Nhã" màu trắng tinh (`text-white`) trên nền khối vát chéo xanh Navy sẫm. Khung ảnh Polaroid chứa ảnh `./screenshots/ava1.png` có độ xoay nghiêng nhẹ tự nhiên. Menu chính hoạt động theo cơ chế One-Page Smooth Scroll bằng ID.

Hãy thực thi viết toàn bộ mã nguồn hoàn chỉnh vào file `index.html` ngay bây giờ.
-----
Nhìn vào bức ảnh chụp lỗi giao diện thực tế `image_196007.jpg` tôi gửi kèm, bạn đang mắc lỗi nghiêm trọng: Ảnh sơ đồ bị phóng to quá cỡ tràn ngập màn hình làm chữ bị vỡ hạt, đồng thời bạn quên hoàn toàn việc chia khối và chèn tiêu đề phụ căn trái `| OVERALL USE CASE DIAGRAM`.

Tôi đã cập nhật lại file `plan.md` đặc tả cấu trúc độc lập. Hãy viết lại toàn bộ vùng nội dung hiển thị trong thẻ Script React cho file `index.html` đáp ứng chính xác các tiêu chuẩn kỹ thuật sau:

1. **Khống chế kích thước và độ hiển thị của ảnh sơ đồ**:
   - Tuyệt đối KHÔNG sử dụng class `w-full` tự do trực tiếp trên thẻ `<img>`.
   - Mỗi file ảnh sơ đồ phải được bọc trong một khung thẻ `div` màu nền trắng (`bg-white`), có viền mỏng (`border border-gray-100`), bo góc lớn (`rounded-xl`), có bóng đổ nhẹ (`shadow-sm`), và lề trong (`p-6`).
   - Thẻ `<img>` bên trong khung phải có class thuộc tính giới hạn chiều cao: `className="max-w-full max-h-[75vh] object-contain mx-auto"` để ảnh tự thu phóng vừa vặn, giữ nguyên độ nét gốc và không bao giờ bị phóng to cưỡng ép.

2. **Tách khối và chèn Tiêu đề phụ căn trái (Strictly Separated Blocks)**:
   - Đối với tab **USE CASE**, bạn không được nhét chung 3 ảnh vào một chỗ. Hãy tạo 3 khối thẻ riêng biệt cách nhau một khoảng dọc (`space-y-16`) căn lề trái (`items-start`).
   - Trước mỗi khung ảnh trắng, bắt buộc phải có một dòng thẻ `div` chứa tiêu đề phụ căn trái, định dạng font chữ Serif, có gạch đứng màu vàng Gold ở đầu y hệt thiết kế:
     * Khối 1: `<div className="border-l-4 border-figmaGold pl-3 font-serif text-lg text-figmaDark font-bold mb-4">| OVERALL USE CASE DIAGRAM</div>` rồi mới đến ảnh `./ai/usecase1.png`.
     * Khối 2: `<div className="border-l-4 border-figmaGold pl-3 font-serif text-lg text-figmaDark font-bold mb-4">| LEVEL 1 USE CASE DIAGRAM</div>` rồi mới đến ảnh `./ai/usecase2.png`.
     * Khối 3: `<div className="border-l-4 border-figmaGold pl-3 font-serif text-lg text-figmaDark font-bold mb-4">| LEVEL 2 USE CASE DIAGRAM</div>` rồi mới đến ảnh `./ai/usecase3.png`.

3. **Áp dụng tương tự cho các Sub-Tabs tài liệu còn lại**:
   - Tab **WORKFLOW**: Có tiêu đề phụ `| WORKFLOW DIAGRAM` trước ảnh `./ai/workflow.png`.
   - Tab **UC SPEC**: Xếp dọc 2 khối, có tiêu đề phụ `| USE CASE SPECIFICATION - PAGE 1` (ảnh `./ai/ucspe1.png`) và `| USE CASE SPECIFICATION - PAGE 2` (ảnh `./ai/ucspe2.png`).
   - Tab **SEQUENCE DIAGRAM**: Xếp dọc 4 khối riêng biệt, có tiêu đề phụ tuần tự từ `| SEQUENCE DIAGRAM 1` đến `4` trước từng ảnh tương ứng từ `./ai/se1.png` đến `./ai/se4.png`.
   - Tab **ERD**: Tiêu đề phụ `| ENTITY RELATIONSHIP DIAGRAM` trước ảnh `./ai/erd.png`.
   - Tab **FIGMA**: Chuỗi tiêu đề phụ từ `| UI/UX PROTOTYPE DESIGN 1` đến `3` trước chuỗi ảnh từ `./ai/fig1.png` đến `./ai/fig3.png`.

4. **Giữ vững UI/UX màn hình chính**: Chữ "Nguyễn Thị" màu vàng gold, chữ "Trang Nhã" màu trắng tinh, khối vát chéo xanh Navy chuẩn góc, khung Polaroid ảnh cá nhân `./screenshots/ava1.png` xoay nghiêng nghệ thuật và cơ chế One-Page Smooth Scroll.

Hãy rà soát và ghi đè lại file `index.html` thật hoàn mỹ cho tôi.