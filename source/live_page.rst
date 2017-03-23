.. wePhone documentation master file, created by
   sphinx-quickstart on Mon Feb 27 18:30:38 2017.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to Live page's documentation!
===================================================

.. toctree::
   :maxdepth: 2
   :caption: Contents:

**********************
1. Bảng điều khiển
**********************

Hiển thị các cuộc gọi trong ngày, số lượng điện thoại viên kết nối, cuộc gọi nhỡ ....

 .. image:: /images/live_page/image_en1.jpg

 Chi tiết các thông số như sau:
 - QoS hôm nay: % Tỷ lệ cuộc gọi được nhận trên tổng số cuộc gọi đến 
 - Gọi nhỡ: Số cuộc gọi nhỡ trong ngày có thể xem chi tiết theo link sau http://wephone-test.localnet.dev/a/samsung.vn#/callcenter/missed_calls
 - Hộp thư thoại: Số thư thoại trong ngày và xem chi tiết theo link sau http://wephone-test.localnet.dev/a/samsung.vn#/voicemail_queue
 - Đang gọi: Hiển thị số cuộc gọi đang thực hiện
 - Đang chờ: Hiển thị số cuộc gọi đang đợi hệ thống tiếp nhận
 - Điện thoại viên đang kết nối: Số lượng điện thoại viên đang kết nối đến tổng đài
 - Điện thoại viên sẵn sàng: Số lượng điện thoại viên hiện đang rảnh
 - Điện thoại viên đang tư vấn: Số lượng điện thoại viên đang thực hiện cuộc gọi
 - Điện thoại viên tạm dừng: Số lượng điện thoại viên đang bận
 - Cuộc gọi trong ngày: Hiển thị biểu đồ số lượng cuộc gọi được xử lý, cuộc gọi nhỡ
 
2. Danh sách cuộc gọi
**********************

Hiển thị danh sách các cuộc gọi đang thực hiện, các tổng đài viên đã kết nối ....

 .. image:: /images/live_page/image_en2.jpg

 Chi tiết các thông số như sau:
  - Lọc theo nhóm: Hiển thị cửa sổ cho phép lựa chọn hiển thị các tổng đài viên trong danh sách các tổng đài viên đã kết nối. 
    .. image:: /images/live_page/image_en3.jpg

  - Lịch sử hành động: Hiển thị cửa sổ các hành động của quản trị viên. Chức năng này chỉ dành cho admin
   .. image:: /images/live_page/image_en4.jpg

  - Tổng đài viên: Trong danh sách các tổng đài viên đã kết nối khi di chuyển chuột qua các tổng đài viên sẽ hiển thị các chức năng như: Ngắt kết nối, tạm dừng, thay đổi hàng đợi cho điện thoại viên, nghe lén, thời gian đã kết nối vào tổng đài, thời gian thực hiện cuộc gọi cuối cùng.


3. Đồ thị
***********
 Thống kê các cuộc gọi đến, cuộc gọi nhỡ bằng biểu đồ theo ngày, tháng năm
 Thống kê các cuộc gọi trong ngày hôm nay như hình bên:
   .. image:: /images/live_page/image_en5.jpg

  Thống kê các cuộc gọi trong ngày hôm qua như hình bên:
   .. image:: /images/live_page/image_en6.jpg

  Thống kê các cuộc gọi trên tuần như hình bên:
   .. image:: /images/live_page/image_en7.jpg

  Thống kê các cuộc gọi tuần này như hình bên:
   .. image:: /images/live_page/image_en8.jpg

  Thống kê các cuộc gọi tháng này như hình bên:
   .. image:: /images/live_page/image_en9.jpg

  Thống kê các cuộc gọi trên tháng như hình bên:
   .. image:: /images/live_page/image_en10.jpg

4. Hàng đợi cuộc gọi
***********
  Hiển thị danh sách hàng đợi với thông tin hiển thị cuộc gọi và tổng đài viên trực tuyến

  .. image:: /images/live_page/image_en11.jpg

5. Cuộc gọi nhỡ
***********
 Thống kê danh sách các cuộc gọi nhỡ trong ngày như hình bên:

  .. image:: /images/live_page/image_en12.jpg

  Chi tiết thống kê các cuộc gọi nhỡ như sau:
  - Ngày bắt đầu: Chọn bất kỳ ngày bắt đầu
  - Ngày kết thúc: Chọn bất kỳ ngày kết thúc 
  - Điện thoại: Nhập số điện thoại
  - Lưu tệp CSV: Tải danh sách các cuộc gọi nhỡ 
  - Danh sách cuộc gọi nhỡ bao gồm: Thời gian gọi, số gọi, số được gọi, hàng đợi, người gọi, gọi lúc, số lần gọi còn lại, trạng thái, thư thoại, thao tác.

6. Cuộc gọi đã xử lý
***********
 Hiển thị danh sách các cuộc gọi đi và cuộc gọi đến trong ngày như hình bên:
 .. image:: /images/live_page/image_en13.jpg

 Chi tiết danh sách các cuộc gọi đã xử lý như sau:
  - Ngày bắt đầu: Chọn bất kỳ ngày bắt đầu
  - Ngày kết thúc: Chọn bất kỳ ngày kết thúc 
  - Điện thoại: Nhập số điện thoại
  - Tổng đài viên: Chọn tổng đài viên muốn xem
  - Lưu tệp CSV: Tải danh sách các cuộc gọi đã xử lý
  - Danh sách cuộc gọi đã xử lý bao gồm: Điện thoại viên đảm nhận, số gọi, số được gọi, gọi ra/gọi vào, thời gian trả lời, thời gian cúp máy, đánh giá, chi tiết đánh giá, thao tác.


Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
