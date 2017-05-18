.. wePhone documentation master file, created by
   sphinx-quickstart on Mon Feb 27 18:30:38 2017.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

How to make a function call
===================================
POST to this URL in order to make a function call: /ws/apikey/call_function
The POST request body should contain a JSON with the following keys:
	- method: The name of the function to call
	- params: A list containing values of argument to the function call

Example of JSON body:
	{
		"method": "did.zone.list_area",
		"params": ["FR", "GEOGRAPHIC"]
	}

Example: /ws/apikey/call_function?apikey=<API KEY OF YOUR ENTERPRISE>


How to obtain the API Key
===================================

You can get the API key from the web interface of wePhone. Click on "Enterprise Information" on the left menu, then "API Integration"

