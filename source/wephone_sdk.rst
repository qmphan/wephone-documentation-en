.. wePhone documentation master file, created by
   sphinx-quickstart on Mon Feb 27 18:30:38 2017.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to Phone number management's documentation!
===================================================

.. toctree::
   :maxdepth: 2
   :caption: Contents:

**********************
1. WEPHONE SDK
**********************

Là thư viện mà wePhone cung cấp để gọi từ bên ngoài nhằm thực thi một số tính năng:
- Liệt kê danh sách người dùng
- ....
 
1.1 Composer
#######################
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
#################################

**Init**
```php
$client = new \WEPHONE\SDK\Client;
$client->init("api-key-code");
```

********************************************************************************


### Người dùng
### Lấy danh các các người dùng

```php
$result = $client->call('user.list_all', array());
```

### Thêm mới một người dùng

```php
$result = $client->call('user.create', array('first', 'last', 'email@domain.com'));
```

### Gỡ bỏ một người dùng

```php
$result = $client->call('user.remove', array('user_public_id'));
```

********************************************************************************


### Số tổng đài
### Lấy danh sách các số 

```php
$result = $client->call('number.list_all', array());
```

### Mua một số

```php
$result = $client->call('number.buy', array('country_code_2letter', 'number_prefix'));
```

### Trả về một số

```php
$result = $client->call('number.return', array('returned_number'));
```

### Định tuyên cho một số

```php
$routingData = array(
    "application"=> "call_phone_number", 
    "params"=> array("number"=> "111")
);
$result = $client->call('number.set_route', array('routed_number', $routingData));


********************************************************************************


### Hàng đợi
### Lấy danh sách của hàng đợi

```php
$result = $client->call('queue.list_all', array());
```



Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
