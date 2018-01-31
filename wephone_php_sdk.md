---
title: Hello
---

# WEPHONE PHP SDK

wePhone PHP SDK is a PHP library that allow you to quickly call wePhone APIs. 
To use the wePhone PHP SDK, you need to get the API key for your enterpise. This can be done by clicking on Settings --> API Integration at the botton of the left menu.
 
1. Setting up the library using composer

Using Composer (https://getcomposer.org/) is an easy way to manage PHP project dependency.
Create a composer.json file as bellow, then run composer update:

Here is the content of composer.json::

```JSON
  {
      "name": "TestSMS",
      "repositories": [
          {
              "type": "vcs",
              "url": "https://github.com/wephone-saas/sdk-php.git"
          }
      ],
      "require": {
          "wephone/sdk-php": "dev-master"
      }
  }
```

Add more library dependency to your `composer.json` as needed. Remember to run `composer update` each time composer.json is updated.

Add the next lines to your PHP source file so that it knows how to find wephone SDK:

```
<?php

require 'vendor/autoload.php';
```

1.2 Usage example


### Init

```
$client = new \WEPHONE\SDK\Client;
$client->init("api-key", "https://admin.wephone.io");
```

---

### Send SMS API
### Send an SMS

```
$client = new \WEPHONE\SDK\Client;
$client->init("xxxx", "https://admin.wephone.io");

$result = $client->call('sms.send',
                        array(  "sender" => "MySenderName",
                                "destination" => "+33611111111",
                                "message" => "Hello, how are you?"
                             )
                        );
```


---
