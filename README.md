[Windows 11/10] How to check the Wi-Fi password on your computer


In the Command Prompt window, type the command ( click windows key+r and then write cmd and then click enter )

[Netsh wlan show profile name=”Wi-F name” key=clear]

and then press Enter key.


Fox example: 
Netsh wlan show profile name=”WLAN2_5G2” key=clear
, WLAN2_5G2 is a Wi-Fi name that has been connected currently. 

![image](https://github.com/ensaronal/How-to-check-the-Wi-Fi-password-on-your-computer/assets/96106312/63f77c1b-a353-4fdb-b605-8e862f583b2e)


You can find the Wi-Fi password in the [Key Content] field of Security settings.

![image](https://github.com/ensaronal/How-to-check-the-Wi-Fi-password-on-your-computer/assets/96106312/93f1220f-dc64-46a5-9d26-919710c370a5)



If you want to check all Wi-Fi passwords the computer has ever connected, you can use the following command. Press Enter key after typing this command, you will find the passwords for each Wi-Fi.
[for /f "skip=9 tokens=1,2 delims=:" %i in ('netsh wlan show profiles') do @echo %j | findstr -i -v echo | netsh wlan show profiles %j key=clear]


![image](https://github.com/ensaronal/How-to-check-the-Wi-Fi-password-on-your-computer/assets/96106312/e370f3c8-fa54-4c2a-8711-db03a44e93b7)

