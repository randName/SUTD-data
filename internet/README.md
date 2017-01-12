# Connecting to SUTD networks
```shell
cat network_interfaces >> /etc/network/interfaces
cat wpa_supplicant.conf >> /etc/wpa_supplicant/wpa_supplicant.conf
mv wpa_wired.conf /etc/wpa_supplicant/

# Hashing password for wpa_supplicant
echo -n 'password' | iconv -t utf16le | openssl md4
```


