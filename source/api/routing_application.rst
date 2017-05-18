===================================
Routing Applications
===================================

List of routing applications

- Call Phone Number
    - Application Name: call_phone_number
    - Application params:
        - number:
        	- Type: string
        	- Required: yes

- Put the call to a call queue
    - application: callqueue
    - params:
        - {param_name: queue, param_type: int, param_value: null, default_value: null, required: 1}

- Call a SIP phone
    - application: call_phone
    - params:
        - sipphone_id:
        	- Type: int
        	- Required: yes
        	
- Go to a conference
    - application: conference
    - params:
        - conference:
	        - Type:  int,
	        - Required: yes

- Go to an IVR
    - application: ivr_custom_menu
    - params:
        - id:
        	- Type: int
        	- Required: yes

