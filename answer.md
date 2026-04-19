## PHẦN A — KIỂM TRA ĐỌC HIỂU
### Câu A1  — HTTP & Browser
**1.**

*Tham chiếu: 01_introduction_html_universe.md — Phần: "Cuộc Hành Trình 0.3 Giây Xuyên Đại Dương"*

*Khi gõ https://shopee.vn và nhấn Enter, hành trình dữ liệu diễn ra như sau:*
  1. DNS Lookup: Trình duyệt hỏi "danh bạ" Internet để tìm địa chỉ IP của Shopee → Đi qua các máy chủ DNS trên thế giới để lấy số hiệu IP chính xác.
  2. Thiết lập kết nối (TCP Handshake): Request từ laptop của bạn → qua Router WiFi → nhà mạng (ISP) → chạy xuyên cáp quang biển để đến máy chủ của Shopee → Hai bên "bắt tay" thiết lập kết nối an toàn.
  3. Gửi Request: Trình duyệt gửi thông điệp: "Tôi muốn xem trang chủ Shopee" → Yêu cầu này bay qua hàng ngàn cây số đến Data Center nơi chứa dữ liệu Shopee.
  4. Server xử lý & Response: Server Shopee nhận lệnh → Kiểm tra kho hàng, khuyến mãi → Đóng gói file HTML, CSS, JS rồi gửi ngược lại theo đường cáp quang về máy tính của bạn.
  5. Render: Trình duyệt Chrome nhận được "gói quà" dữ liệu → Bắt đầu phân tích mã nguồn (Parsing) → Dựng khung, tô màu và hiển thị (Render) → Bạn nhìn thấy giao diện Shopee để bắt đầu mua sắm.
   
**2.**
*Thông tin của tab Network:*
1. Danh sách các tài nguyên (Requests)
Khi bạn load một trang web, nó không phải là một file duy nhất. Tab Network sẽ liệt kê tất cả các file được tải về như: file HTML, file ảnh (JPG, PNG), file định dạng (CSS), file xử lý (JS), hay các lời gọi API.

3. Trạng thái phản hồi (Status Code)
   
--- Đây là cột cực kỳ quan trọng giúp bạn biết request đó có thành công hay không:

200 OK: Tải thành công.

404 Not Found: File không tồn tại (ví dụ link ảnh bị hỏng).

500 Internal Server Error: Lỗi từ phía máy chủ.

3. Loại file (Type)

Cột này phân loại dữ liệu để bạn dễ quản lý, ví dụ: document (HTML), stylesheet (CSS), script (JS), png/jpeg (Ảnh).

4. Thời gian tải (Time & Waterfall)
   
Time: Tổng thời gian để tải xong một file cụ thể.

Waterfall: Một biểu đồ hình thác nước cho thấy trình tự file nào tải trước, file nào tải sau và chúng có bị "nghẽn" ở đâu không.

5. Kích thước (Size)

Cho biết file đó nặng bao nhiêu (KB/MB). Điều này giúp các lập trình viên biết được tại sao trang web của họ bị chậm (thường là do ảnh quá nặng).



