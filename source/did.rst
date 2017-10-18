.. wePhone documentation master file, created by
   sphinx-quickstart on Mon Feb 27 18:30:38 2017.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to Phone number management's documentation!
===================================================

.. toctree::
   :maxdepth: 2
   :caption: Contents:

**************
1. WEPHONE SDK
**************

Là thư viện mà wePhone cung cấp để gọi từ bên ngoài nhằm thực thi một số tính năng:
- Liệt kê danh sách người dùng
- ....
 
1.1 Composer
#############
Sử dụng Composer (https://getcomposer.org/) để quản lý các PHP dependencies.
Nếu chưa có `composer.json`, tạo một file ở thư mục root của project, tải về Composer, & chạy `composer update`.

Tệp `composer.json` được config như dưới đây:
```json
{
    "name": "wephone/sdk-php",
    "autoload": {
        "psr-0" : {
            "WEPHONE" : "src"
        }
    }
}
```

Thêm các thư viện khác cho project của bạn trong `composer.json`. Đừng quên chạy `composer update` mỗi khi sửa tệp.

Sau đó thêm các dòng sau vào code:
```php
<?php

require 'vendor/autoload.php';
```

1.2 Cách sử dụng
################

**Init**
```php
$client = new \WEPHONE\SDK\Client;
$client->init("api-key-code");
```

********************************************************************************


### Số điện thoại tổng đài
### Lấy danh các các quốc gia hỗ trợ mua số tổng đài

```php
$result = $client->call('did.zone.list_country', array());
```

### Lấy danh các các khu vực (thuộc quốc gia) hỗ trợ mua số tổng đài

```php
$result = $client->call('did.zone.list_area', array('country_code_2letter', 'type')); 
//type phải là ('GEOGRAPHIC', 'NATIONAL', 'MOBILE')
```

ví dụ: 

```php
$result = $client->call('did.zone.list_area', array('FR', 'GEOGRAPHIC'));
```


### Mua số tổng đài

```php
$result = $client->call('did.reserve', array('area_code_id', 'quantity', 'mode', 'class')); 
//mode phải là ('RANDOM', 'SEQUENTIAL')
//class phải là ('CLASSIC', 'GOLD')
```

ví dụ: 

```php
$result = $client->call('did.reserve', array(2, 2, 'RANDOM', 'CLASSIC'));
```


********************************************************************************



Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
