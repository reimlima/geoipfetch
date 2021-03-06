# geoipfetch
--------------------------------------------------------------------------------

Geo Localization from a Given IP Address or Site URL

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
* **26/07/2017 - v2.1**
Handling with "no command line parameter given"
* **31/07/2017 - v2.2**
Handling with "no command line parameter given"
* **09/08/2017 - v2.3**
Search in geoipfetch.net and/or ip-api.com in a single function
* **31/08/2017 - v2.4**
Bug Fix - Handling with numbers in site url.

# How to use it
--------------------------------------------------------------------------------

Example:

```sh

# Usage

$ geoipfetch 
No Address or IP given

Usage: give a valid URL or IP Address, like:

        geoipfetch https://www.google.com
OR
        geoipfetch 216.58.222.3

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
