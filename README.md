[Windows 11/10] How to check the Wi-Fi password on your computer

If you forgot the Wi-Fi password of existing networks on your computer, this article describes two methods to check the password.

In the Command Prompt window, type the command ( click windows key+r and then write cmd and then click enter )
![image](https://github.com/ensaronal/How-to-check-the-Wi-Fi-password-on-your-computer/assets/96106312/63f77c1b-a353-4fdb-b605-8e862f583b2e)

[Netsh wlan show profile name=”Wi-F name” key=clear]

and then press Enter key.


Fox example: 
Netsh wlan show profile name=”WLAN2_5G2” key=clear
, WLAN2_5G2 is a Wi-Fi name that has been connected currently. 

