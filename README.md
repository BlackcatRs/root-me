# root-me
------------

1. HTTP - IP restriction bypass

------------
## Challenge

### HTTP - IP restriction bypass
  *Only local users will be able to access the page*

### Vulnerability

Some web application use ip address to block access to the visitors. this is the case for some administrator interfaces.

To implement this, the web application will check the `REMOTE_ADDR` value that the web server passes through to the application.

If the visitor is using a proxy, the `REMOTE_ADDR` field will contain the address of the proxy instead of the visitor. So some proxy add `X-Forwarded-For` to be able to see the visitor's ip address by web server.


### Exploit
So, we need to use this method to say that i am a client of you network.

### Requirements
- Python3

### Execute
`python3 IP_restriction_bypass.py`
------------
