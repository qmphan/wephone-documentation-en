.. wePhone documentation master file, created by
   sphinx-quickstart on Mon Feb 27 18:30:38 2017.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to User management's documentation!
===========================================

.. toctree::
   :maxdepth: 2
   :caption: Contents:

*********************
1. Tạo mới người dùng
*********************

1.1. Tạo mới người dùng từ giao diện Web
########################################
 Từ giao diện chọn Thêm mới để hiển thị giao diện thêm mới người dùng như sau.
  .. image:: /images/user/image_en1.jpg 

 Nhập thông tin người dùng như sau:
    - Họ &Tên đệm: Họ và tên đệm của Điện thoại viên
    - Tên: Tên của Điện thoại viên
    - Email: Địa chỉ hòm thư điện tử của Điện thoại viên
    
1.2 Nhập danh sách người dùng từ tệp tin csv
############################################
 Chọn Nhập tài khoản từ tệp tin để hiển thị giao diện như sau.
  .. image:: /images/user/image_en2.jpg  

 Thông tin giao diện như sau:
    - Tải về file mẫu: Click vào link này sẽ tải về file mẫu để nhập thông tin người dùng
    - Gửi mail cho từng người sử dụng với thông tin tài khoản: Lựa chọn này cho phép gửi Tên tài khoản và Mật khẩu về email của người dùng.
    - Kéo thả hoặc nhấn vào đây để tải tệp: Click vào link này để tải file đã nhập thông tin người dùng.

***************************************
2. Kết nối một SIP phone cho người dùng
****************************************
 Chọn Bật VOIP để hiển thị giao diện SIP phone như sau.
  .. image:: /images/user/image_en3.jpg  

 Thông tin giao diện như sau:
    - Số extension WePhone: Được sử dụng để cài đặt trên Softphone và thực hiện các cuộc gọi ra, vào của hệ thống WePhone
    - Số DID dành riêng: Là đầu số được chỉ định dành riêng cho 1 Điện thoại viên, khi gọi tới đầu số này thì cuộc gọi chỉ được định tuyến tới Điện thoại viên đó
    - Cho phép gọi qua IP Phone: Cho phép ĐTV gọi ra với các tùy chọn.
        - Định danh số gọi ra: Khi gọi ra thì sử dụng số này để thực hiện cuộc gọi
        - Gọi trực tiếp, Cho phép sử dụng số gọi ra để gọi ra 1 cách trực tiếp, có 3 lựa chọn: Cho phép gọi ra quốc tế, cho phép gọi trong nước & cả 2.
        - Gọi qua tổng đài: Cho phép sử dụng số gọi ra để gọi ra thông qua 1 hàng đợi.
    - Thông tin kết nối: Đây là thông tin cấu hình cho SipPhone thông qua các SoftPhone (3CX, X-Lite, Zoiper).


Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
