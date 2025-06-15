# Tra cứu Phường/Xã tại TP.HCM Sau Sáp Nhập

Đây là một ứng dụng web đơn giản, một trang duy nhất giúp người dân tại Thành phố Hồ Chí Minh tìm kiếm thông tin về phường hoặc xã mới của mình sau đợt điều chỉnh địa giới hành chính toàn thành phố. Người dùng có thể tìm kiếm bằng tên phường/xã cũ hoặc mới, hoặc sử dụng vị trí GPS hiện tại để xác định đơn vị hành chính mới của mình.

Ứng dụng sẽ hiển thị thông tin chi tiết về phường/xã mới, bao gồm tên, các đơn vị cũ được sáp nhập, thông tin dân số, diện tích, mật độ dân số, và vị trí trụ sở hành chính mới trên bản đồ tương tác.

## Tính năng ✨

* **Tìm kiếm theo tên**: Tìm phường/xã mới của bạn bằng cách nhập tên đơn vị hành chính cũ hoặc mới.
* **Định vị GPS**: Sử dụng vị trí hiện tại của thiết bị để tự động xác định phường/xã bạn đang ở.
* **Bản đồ tương tác**: Xem ranh giới của phường/xã mới trên bản đồ tương tác, được cung cấp bởi LeafletJS và Google Maps.
* **Thông tin chi tiết**: Nhận các số liệu thống kê quan trọng về đơn vị hành chính mới của bạn, bao gồm:
    * Tổng dân số và thứ hạng toàn thành phố.
    * Tổng diện tích (tính bằng km²) và thứ hạng toàn thành phố.
    * Mật độ dân số và thứ hạng toàn thành phố.
    * Danh sách các phường/xã cũ đã được sáp nhập.
    * Danh sách các phường/xã giáp ranh.
    * Địa chỉ trụ sở hành chính mới.
* **Chỉ đường**: Nhận liên kết đến Google Maps để xem chỉ đường đến trụ sở hành chính mới.
* **Cá nhân hóa (Tùy chọn)**: Người dùng có thể thêm tên và ảnh để kết quả hiển thị được cá nhân hóa hơn. Thông tin này được xử lý hoàn toàn phía trình duyệt và không được lưu trữ hay thu thập.
* **Thiết kế tương thích**: Giao diện được thiết kế để hoạt động tốt trên cả máy tính để bàn và thiết bị di động.

## Công nghệ sử dụng 💻

* **Giao diện người dùng**: HTML, [Tailwind CSS](https://tailwindcss.com/)
* **Thư viện JavaScript**:
    * [LeafletJS](https://leafletjs.com/): Dùng cho bản đồ tương tác.
    * [Font Awesome](https://fontawesome.com/): Dùng cho các biểu tượng (icons).
* **Dữ liệu**:
    * GeoJSON cho dữ liệu ranh giới hành chính. Dữ liệu gốc từ [OpenStreetMap](https://www.openstreetmap.org/), xử lý bằng [Atlas](https://atlas.co)
    * TSV cho dữ liệu thống kê.
* **Fonts**: [Google Fonts](https://fonts.google.com/) (Inter)

## Hướng dẫn sử dụng 🚀

1.  Mở tệp `index.html` trong trình duyệt web của bạn.
2.  **Để tìm kiếm theo tên:**
    * Nhập tên của một phường hoặc xã (cũ hoặc mới) vào ô tìm kiếm.
    * Nhấp vào nút tìm kiếm hoặc nhấn phím Enter.
    * Nếu tìm thấy nhiều kết quả, một danh sách sẽ được hiển thị. Nhấp vào kết quả đúng để xem chi tiết.
3.  **Để sử dụng vị trí của bạn:**
    * Nhấp vào nút "Dùng vị trí hiện tại của tôi".
    * Cho phép trình duyệt truy cập vị trí của bạn khi được yêu cầu.
    * Ứng dụng sẽ tự động tìm và hiển thị thông tin cho phường/xã hiện tại của bạn.
4.  **(Tùy chọn)** Thêm tên của bạn và tải lên một bức ảnh để cá nhân hóa thẻ kết quả.

## Nguồn dữ liệu 📊

* Dữ liệu ranh giới hành chính (GeoJSON) và thông tin thống kê (TSV) được tổng hợp từ các nguồn tin tức công khai và các thông báo chính thức liên quan đến việc sáp nhập.
* Dữ liệu được lưu trữ trên một kho mã nguồn mở GitHub. Để biết thêm chi tiết hoặc tải xuống dữ liệu, vui lòng tham khảo liên kết liên hệ ở chân trang của ứng dụng.

## Miễn trừ trách nhiệm ⚠️

Đây là một dự án cá nhân được tạo ra chỉ nhằm mục đích cung cấp thông tin. Dữ liệu được dựa trên thông tin công khai và có thể không chính xác hoặc cập nhật 100%. Ứng dụng không thu thập hoặc lưu trữ bất kỳ dữ liệu cá nhân nào của người dùng.

## Mời mình một ly cafe ☕
<img src="https://raw.githubusercontent.com/lqtue/phuongnao/main/qr-code.jpg" alt="Mã QR ủng hộ" class="mx-auto w-52 h-52 rounded-lg border-2 border-gray-200" onerror="this.alt='Không tìm thấy ảnh QR'; this.src='https://placehold.co/208x208/e0e0e0/757575?text=QR+Code';">
