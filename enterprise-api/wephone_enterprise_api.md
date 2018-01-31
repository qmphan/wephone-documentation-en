---
Title: wePhone Enterprise API
---

## Phone Number API
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

