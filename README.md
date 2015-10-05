# sgrep -- Section grep

`sgrep` works in the same way `grep` works, but prints the descendant lines also. Descendant lines are the indented lines below the matched line. 

If `-p` parameter is given as the first parameter, then the parent section is also printed. 

Usage example: 

    # to get my_ssid's quality: 

    iwlist wlan0 scan | sgrep my_ssid -p | sgrep Quality


    # to get wlan0's all information: 
    ifconfig | sgrep wlan0
