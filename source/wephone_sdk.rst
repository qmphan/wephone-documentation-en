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
1. WEPHONE PHP SDK
**********************

wePhone PHP SDK is a PHP library that allow you to quickly call wePhone APIs. 
To use the wePhone PHP SDK, you need to get the API key for your enterpise. This can be done by clicking on Settings --> API Integration at the botton of the left menu.
 
1.1 Setting up the library using composer
#######################
Using Composer (https://getcomposer.org/) is an easy way to manage PHP project dependency.
Create a composer.json file as bellow, then run composer update:

Here is the content of composer.json

```
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
#################################

**Init**

```
$client = new \WEPHONE\SDK\Client;
$client->init("api-key-code", "https://admin.wephone.io");
```

********************************************************************************

### User management
### Get user list

```
$result = $client->call('user.list_all', array());
```

### Add a new user

```
$result = $client->call('user.create', array('first', 'last', 'email@domain.com'));
```

### Remove an user

```
$result = $client->call('user.remove', array('user_public_id'));
```

********************************************************************************

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


********************************************************************************

### Phone Number API
### Get the list of enterprise DID

```
$result = $client->call('number.list_all', array());
```

### Buy a phone number


```
$result = $client->call('number.buy', array('country_code_2letter', 'number_prefix'));
```

### Return a phone number


```
$result = $client->call('number.return', array('returned_number'));
```

### Define call routing for a phone number


```
$routingData = array(
    "application"=> "call_phone_number", 
    "params"=> array("number"=> "111")
);
$result = $client->call('number.set_route', array('routed_number', $routingData));
```

********************************************************************************

### Call queue
### Get the list of all call queues

```
$result = $client->call('queue.list_all', array());
```


Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
