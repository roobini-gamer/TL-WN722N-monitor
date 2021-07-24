this project is a fork from aircrack-ng/rtl8188eus


# tutorial describes how to enable monitor mode in TP-LINK TL-WN722N V2/V3 in KALI LINUX



# Supports
* Android 7
* MESH Support
* Monitor mode
* Frame injection
* Up to kernel v5.8+
... And a bunch of various wifi chipsets

# Howto build/install
1. `sudo apt update`
2. `sudo apt install bc`
3. `sudo rmmod r8188eu.ko`
4. `git clone https://github.com/roobini-gamer/TL-WN722N-monitor`
5. `cd rtl8188eus`
6. `sudo -i`
7. `echo "blacklist r8188eu" > "/etc/modprobe.d/realtek.conf"`
8. `exit`
9. `make`
10. `sudo make install`
11. `sudo modprobe 8188eu`


# MONITOR MODE howto
Use these steps to enter monitor mode.
```
$ ifconfig wlan0 down
$ airmon-ng check kill
$ iwconfig wlan0 mode monitor
$ ifconfig wlan0 up
$ iwconfig
```


# Credits
Realtek       - https://www.realtek.com<br>
Alfa Networks - https://www.alfa.com.tw<br>
aircrack-ng.  - https://www.aircrack-ng.org<br>
contributors  - https://github.com/aircrack-ng/rtl8188eus/graphs/contributors<br>

