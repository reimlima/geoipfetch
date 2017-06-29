# geoipfetch
--------------------------------------------------------------------------------

Geo Localization from a Given IP Address

# Notice
--------------------------------------------------------------------------------

* This script was tested and work well in Python 2.7.6

* This script depends to the access to 'api.geoiplookup.net' and/or 'ip-api.com'

# Changelog
--------------------------------------------------------------------------------
* **28/06/2017 - v1**
First Stable Release
* **29/06/2017 - v2**
Now work with site url.

# How to use it
--------------------------------------------------------------------------------

Example:

```sh

# Search by IP

$ geoipfetch 216.58.222.3
IP: 216.58.222.3
Hosted by: Google
City: Mountain View
Country: United States

# Search by Site URL ...

$ geoipfetch https://www.google.com.br
IP: 216.58.222.3
Hosted by: Google
City: Mountain View
Country: United States

# ... with or without 'http://' or 'https://'... 

$ geoipfetch www.google.com.br
IP: 216.58.222.3
Hosted by: Google
City: Mountain View
Country: United States

# ... even with 'query strings'

$ geoipfetch https://www.google.com.br/?gws_rd=ssl#safe=off\&q=python
IP: 216.58.222.3
Hosted by: Google
City: Mountain View
Country: United States

# Validate if the Address is really a thing

$ geoipfetch www.thegoogle.com.br
Invalid Address

# And if it's a valide IP Address

$ geoipfetch 256.58.222.3
Invalid IP Address
```
