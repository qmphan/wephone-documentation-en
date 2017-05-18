*************************************
Functions for buying phone numbers
*************************************


====

did.zone.list_country
---------------------

Get the list of countries you can buy phone number from.

**Parameters:**
    No parameter

**Result:**
	This function returns a JSON object. The attribute "country_list" contain the country list. For example:

	.. code-block:: json

		{
			"country_list": [
				{
					"country_name": "FRANCE",
					"code": "FR"
				},
				{
					"country_name": "United States",
					"code": "US"
				}
			]
		}

======

did.zone.list_area
------------------

Get areas list in a country

**Parameter:**
	- country_code: The country code
	- did_type: DID Type. Can take one of the following values: GEOGRAPHIC, NATIONAL, MOBILE

**Result:**
	The list of areas from which you can buy phone numbers.


======
did.reserve
------------------


**Parameter:**
    - area_code_id (int): The id of the area
    - quantity (int): The number of DID to add to the shopping cart.
    - mode  (string): NOT USED FOR NOW (RANDOM or SEQUENTIAL in the future)
    - class (string): Type of DID to buy


**Result:**
	This function add one or multiple DID into the current order if exists. Otherwise, it will create a new order.
    Example of return value:
    {
		"token": "(string)", // ID of the current order
		"expire": "2017-04-24 00:42:42", // Expiration date
		"items": [] // List of DID numbers currently in the order
	}


======
did.order.pay
------------------

	Valid an order and pay for it.

**Parameter:**
	- order_token: The token returned by the function did.reserve

**Result:**
	Information on whether the payment has succeeded
