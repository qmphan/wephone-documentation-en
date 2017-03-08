.. wePhone documentation master file, created by
   sphinx-quickstart on Mon Feb 27 18:30:38 2017.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to Call queue management's documentation!
=================================================

.. toctree::
   :maxdepth: 2
   :caption: Contents:

******************
1. Hàng đợi là gì?
******************
 Hàng đợi là quản lý các cuộc gọi đến từ các khách hàng hoặc gọi đi từ điện thoại viên. Một hàng đợi bao gồm một nhóm các điện thoại viên xử lý cuộc gọi của khách hàng trong hàng đợi.

 Hệ thống này cho phép chuyển tiếp một số cuộc gọi đang chờ cho điện thoại viên tiếp theo trong hàng đợi. Các cuộc gọi được chuyển hướng đến các điện thoại viên đầu tiên có sẵn để giảm sự chờ đợi của khách hàng.

 Giao diện hàng đợi sẽ được hiển thị như sau:
  .. image:: /images/call_queue/image_en1.jpg 

***********************
2. Tạo mới một Hàng đợi
***********************
 Để tạo mới hàng đợi, người dùng nhấn nút "Tạo mới" sau đó hiển thị 1 cửa sổ:
  .. image:: /images/call_queue/image_en2.jpg 

2.1. Giao diện Tổng quan
########################  

   .. image:: /images/call_queue/image_en3.jpg 
   Nhập thông tin như sau:
    - Logo: Logo của hàng đợi, dễ dàng cho việc nhận biết đối với người sử dụng.
    - Tên: Nhập tên của hàng đợi.
    - Nhóm: Chọn nhóm điện thoại viên tham gia vào hàng đợi.
    - Giờ mở cửa: Chọn giờ mở cửa của hàng đợi mà khách hàng có thể gọi đến. Ngoài những giờ này các cuộc gọi của khách hàng sẽ được chuyển vào hộp thư thoại. Điện thoại viên có thể tùy chỉnh giờ làm việc bằng cách nhấn vào nút "Tạo mới" . Một cửa sổ "Tạo một giờ mở cửa mới" sẽ mở ra và sẽ nhắc điện thoại viên điền các thông tin cần thiết cho các tuỳ biến của giờ mở cửa mới.
    - Ghi âm từ hàng đợi: Chọn kích hoạt hoặc vô hiệu hóa ghi âm cuộc gọi cho phép điện thoại viên nghe các lại các cuộc gọi từ khách hàng trong tranh chấp hoặc khiếu nại của khách hàng.
    - Hộp thư thoại: Người gọi đến có thể để lại tin nhắn trong trường hợp không có điện thoại viên trả lời.
    - Gửi tin nhắn bằng email tới các địa chỉ sau: Người sử dụng cài đặt các địa chỉ email để nhận các tin nhắn thoại.
    - Mức ưu tiên: Có các mức Rất cao, Cao, Trung bình, Thấp, Rất thấp dành cho mức ưu tiên của hàng đợi. Độ ưu tiên cao thì được xử lý trước.

2.2. Giao diện Âm thanh hàng đợi
################################
   
   .. image:: /images/call_queue/image_en4.jpg 
  Nhập thông tin như sau:
   - Ngôn ngữ: Cho phép hỗ trợ đa ngôn ngữ cho các thông điệp trong hàng đợi. Chọn ngôn ngữ  người dùng muốn kích hoạt các hàng đợi.
   - Lời chào: Chọn tin nhắn chào mừng các khách hàng nghe thấy khi thực hiện một cuộc gọi.
   - Nhạc chờ kết nối: Chọn nhạc chờ cho khách hàng trong lúc chờ kết nối đến điện thoại viên.
   - Nhạc chờ giữ máy: Chọn nhạc chờ cho khách hàng trong lúc chờ đợi giữa cuộc gọi.
   - Thông báo khi gọi ngoài giờ làm việc: Chọn tin nhắn thông báo ngoài giờ làm việc của hàng đợi.
   - Thông báo khi không có điện thoại viên nào rảnh: Chọn thông báo đến khách hàng khi trong hàng đợi các điện thoại viên đều bận.

2.3. Giao diện Khi cuộc gọi kết thúc
####################################
   
   .. image:: /images/call_queue/image_en5.jpg 

  Là các hành động được thực thi sau khi kết thúc cuộc gọi.
   - Lựa chọn Menu: Người sử dụng chọn các menu có sẵn để thực hiện tiếp sau khi kết thúc cuộc gọi.
   - Lý do tạm dừng: Điện thoại viên sẽ có khoảng thời gian tạm dừng để thực hiện các việc chuyên môn đối với cuộc gọi vừa gọi.
   - Tổng đài viên trở lại khả dụng sau (giây): Sau mỗi cuộc gọi người sử dụng cài đặt chế độ sau bao nhiêu lâu tổng đài viên có thể tiếp nhận cuộc gọi khác.

2.4. Giao diện Phân loại cuộc gọi
#################################
   
   .. image:: /images/call_queue/image_en6.jpg 

  Là việc đánh giá nhằm phân loại khách hàng, để sử dụng cho việc thống kê sau này.
   - Kích hoạt phân loại cuộc gọi: Sau mỗi cuộc gọi sẽ hiển thị tính năng đánh giá
   - Cuộc gọi vào: Phân loại các cuộc gọi vào
   - Cuộc gọi ra: Phân loại các cuộc gọi ra

2.5. Giao diện Hành động của Back-office
########################################
   
   .. image:: /images/call_queue/image_en7.jpg 

  Tùy chọn này cho phép hiển thị ra giao diện mỗi khi có cuộc gọi đến dựa trên số điện thoại gọi tới. Có 3 tùy chọn:
   - Không làm gì: Lựa chọn này sẽ không hiển thị thông tin gì trên trang back-office.
   - Mở danh bạ: Lựa chọn này sẽ hiển thị form tạo mới hoặc cập nhật thông tin của khách hàng đang gọi đến.
   - Mở trang URL: Người sử dụng nhập ô text có external url có dạng: https://external-url.domain?called_number=$called_number$&calling_number=$calling_number$. Trong đó $called_number$ là số gọi tới, $calling_number$ là số gọi đi 

2.6. Giao diện Chuyển hướng cuộc gọi
####################################
   
   .. image:: /images/call_queue/image_en8.jpg 

  Là các số được định ra dành cho việc chuyển tiếp cuộc gọi. Các số này sẽ là lựa chọn khi điện thoại viên muốn chuyến tiếp 1 cuộc gọi.

********************************
3.  Thêm người dùng vào Hàng đợi
********************************

Cho phép người dùng xem danh sách các điện thoại viên hiện có trong hàng đợi. Chỉ các điện thoại viên nằm trong danh sách này mới được tham gia nhận cuộc gọi đến hoặc đi từ hàng đợi này.
  .. image:: /images/call_queue/image_en9.jpg 

*********************************
4. Định tuyến một số đến Hàng đợi
*********************************
Số DID định tuyến dành riêng cho hàng đợi này được sử dụng để gọi vào và gọi ra. Khách hàng sẽ gọi đến doanh nghiệp thông qua số DID này. Các điện thoại viên có thể lựa chọn số DID này để gọi ra khách hàng.
  .. image:: /images/call_queue/image_en10.jpg 


Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
