## CONNECTING TO WIFI:
You need iwlwifi-MVM NOT dwm.  
After you install libell and iwlwifi-MVM, copy the iwd config file to /etc/iwd.  

`systemctl enable iwd.service`  
`systemctl start iwd.service`  
iwctl, then iwd prompt appears : [iwd]#  
`device list`  
`station [wifi device name] scan`  
`station " " get-networks`  
`station " " connect "SSID"` ( you need to use double quotes if there are spaces in the SSID name)  
NOW YOU SHOULD HAVE WIFI. ENJOY!!

