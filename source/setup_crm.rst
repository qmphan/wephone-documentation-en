.. wePhone documentation master file, created by
   sphinx-quickstart on Mon Feb 27 18:30:38 2017.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to Setup CRM's documentation!
===================================================

.. toctree::
   :maxdepth: 2
   :caption: Contents:

********************
1. Giới thiệu chung
********************

- C-R-M là viết tắt của Customer Relationship Management_ Quản lý quan hệ khách hàng.
- CRM là thuật ngữ dùng để chỉ các thực tiễn, chiến lược và công nghệ mà các công ty sử dụng để quản lý và phân tích tương tác dữ liệu của khách hàng trong suốt vòng đời của khách hàng nhằm mục đích cải thiện mối quan hệ kinh doanh với khách hàng, hỗ trợ duy trì khách hàng và thúc đẩy phát triển doanh số bán hàng. 
- Các hệ thống CRM được thiết kế để thu thập thông tin về khách hàng qua các kênh khác nhau hoặc các điểm tiếp xúc giữa khách hàng và công ty bao gồm trang web của công ty, điện thoại, chat trực tiếp, thư trực tiếp, tài liệu tiếp thị và phương tiện truyền thông xã hội. Các hệ thống CRM cũng có thể cung cấp cho nhân viên những thông tin chi tiết về thông tin cá nhân của khách hàng, lịch sử mua hàng, sở thích mua hàng và các mối quan tâm.

***************
2. Cài đặt CRM
***************
 
Người dùng lựa chọn  Setup, my account 
  .. image:: /images/setup_crm/image01_en.jpg  

Lựa chọn Two Factor Authentication sẽ hiển thị như sau:
 .. image:: /images/setup_crm/image02_en.jpg 

Chọn Application Specific Passwords để tạo các ứng dụng độc lập như ứng dụng thư khách POP/ IMAP/ Outlook, Jabber Chat, v.v. Người dùng cần mật khẩu dành riêng cho ứng dụng để đăng nhập vào các ứng dụng đó.

  .. image:: /images/setup_crm/image03_en.jpg 

  - Tên thiết bị hoặc ứng dụng
  - Mật khẩu hiện tại

Zoho sẽ tự động tạo ra một chuỗi mật khẩu như sau:
  .. image:: /images/setup_crm/image04_en.jpg 

Sau khi có chuỗi mật khẩu người dùng thay các thông số trong đường dẫn sau và chạy Postman để có Authtoken.
https://accounts.zoho.com/apiauthtoken/nb/create?SCOPE=ZohoCRM/crmapi&EMAIL_ID=[Username/EmailID]&PASSWORD=[Password]&DISPLAY_NAME=[ApplicationName]
Các  tham số được truyền đi cùng với URL này là:
- Email_ID: Tên người dùng hoặc ID Email Zoho CRM
- Scope: Chỉ giá trị như ZohoCRM/crmapi
- Password: Mật khẩu Zoho CRM của người dùng
- Display_name: Tên ứng dụng mô tả mục đích sử dụng AuthToken này. Ví dụ "WePhone" hoặc "Google Apps"
Chạy URL này vào Postman, người dùng sẽ được Authtoken như sau:

  .. image:: /images/setup_crm/image05_en.jpg 

Đăng nhập vào trang Wephone ->Enterprise information -> Enterprise CRM
  .. image:: /images/setup_crm/image06_en.jpg 

- Name: Tên ứng dụng
- Type: Có 2 lựa chọn: Zoho CRM, VTiger
- URL: Nhập đường dẫn hiển thị thông tin khách hàng
- API Key: Nhập AuthToken đã được tạo ở Postman
Thực hiện cuộc gọi thông tin khách hàng sẽ hiển thị trên giao diện người dùng như sau:
 
 .. image:: /images/setup_crm/image07_en.jpg





Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
