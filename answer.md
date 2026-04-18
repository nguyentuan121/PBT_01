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

