.. wePhone documentation master file, created by
   sphinx-quickstart on Mon Feb 27 18:30:38 2017.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to Eavesdrop's documentation!
=====================================

.. toctree::
   :maxdepth: 2
   :caption: Contents:

*********************
1. Nghe lén là gì?
*********************
 
 Chức năng này cho phép người dùng có thể đồng thời nghe được các cuộc gọi đang diễn ra của điện thoại viên và khách hàng. Chức năng này chỉ dành riêng cho admin và supervisor.

******************************************************************************
2. Các loại đối tượng có thể nghe lén và thứ tự các cuộc gọi sẽ được thực hiện
******************************************************************************

  2.1. Các loại đối tượng có thể nghe lén
  #######################################
    Có 3 loại đối tượng có thể nghe lén
     - User
      - Hàng đợi
      - Nhóm

  2.2.  Thứ tự các cuộc gọi sẽ được thực hiện
  ############################################
  Để thiết lập nghe lén, chọn nút "Nghe lén" sau đó hiển thị cửa sổ nghe lén như sau.
    .. image:: /images/eavesdrop/image_en1.jpg  

    Khi có cuộc gọi đến điện  thoại viên sẽ nhận cuộc gọi đồng thời cuộc gọi cũng được chuyển đến số Sip Phone của admin hoặc supervisor. Lúc này, admin hoặc supervisor có thể thực hiện nghe lén cuộc gọi.

***************************
3. Làm cách nào để nghe lén.
****************************
  3.1. Đối với cuộc gọi đang hoạt động
  ####################################
  Cuộc gọi đang hoạt động, quản trị viên có thể chọn nút nghe lén trên giao diện "Các cuộc gọi đang thực hiện" như sau
    .. image:: /images/eavesdrop/image_en2.jpg  

  Khi đó cửa sổ nghe lén hiển thị và nhập số sipphone như sau.
   .. image:: /images/eavesdrop/image_en3.jpg  

  Cuối cùng, cuộc gọi được chuyển đến số Sipphone của admin hoặc supervisor

  3.2. Đối với một điện thoại viên
  ################################
  Đối với mỗi điện thoại viên trên danh sách "Các tổng đài viên đã kết nối" đều có chức năng nghe lén. Sau khi chọn nút "nghe lén" sẽ hiển thị cửa sổ nghe lén.
    - Đối với nghe lén một lần, chọn nút "nghe lén một lần" như sau.
      .. image:: /images/eavesdrop/image_en1.jpg  

    - Đối với nghe lén tới khi là nghe lén tất cả các cuộc gọi trong thời gian đã chọn, Chọn nút " nghe lén tới khi" như sau.
      .. image:: /images/eavesdrop/image_en4.jpg  




Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
