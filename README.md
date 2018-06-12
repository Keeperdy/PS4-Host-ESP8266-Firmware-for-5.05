# NB!!! STOLEN CODE FROM C0d3m4st4
Hi, guys! Concerning situation with c0d3m4st4 code used in my ESP firmwares - he blames me his code being stolen and used by me - I want to make it clear that it's just **a stupid mistake,** specifically, my mistake that I did not clear ESP flash memory before uploading any sketch in it. However, I've just found this function, too late. So, if you use somebody's firmware and then upload your sketch via Arduino (Not NodeMCU-flasher) over it, it will replace only sketch code and allocate SPIFF files in flash memory according to their size. The rest is unchanged, so if you firmware is smaller than all 4Mb, you can find the traces of previously loaded firmwares to ESP code! 

My firmware is written from the scracth, using Arduino in-built examples and modified by me!!! **I NEVER TOOK OR STOLE ANYONE'S WORK TO PRESENT IT LIKE MY OWN!!!**

I made a video of a full process where you can see how it works! Video: https://drive.google.com/open?id=1_Drp0A0sBM5yU9vVWsz9NjdxsnubvqVm … The file is over 700 Mb with step-by-step comments.

1. Flashing ESP with blank 4mb bin file 
2. Uploading my sketch and dump bin file 
3. Checking it in WinHex (it crashes sometimes) for c0d3m4st4's code 
4. Flashing ESP with his last FW 
5. Upload again the SAME sketch without erasing the content and dumping a bin file 
6. Finding with WinHex the pieces of his code!!!

Now I will clear all my firmwares from c0d3m4st4's code traces (and probably other devs too) and update them on Github!!! Sorry for inconveniences!!!


**PS4-Host-ESP8266-Firmware OFW 5.05/Прошивка для ESP8266 PS4 Хост (ПО 5.05) (описание на русском смотрите внизу)**
***
Here you can find ESP8266 custom firmware for hosting PS 4 payloads for 5.05 OFW ONLY. It is simple and light firmware without any tools like autopayload, firmware upgrade, ftp server for uploading files, etc. T

The payloads list includes:

    MIRA+HEN
    Xvortex's HEN v1.6
    Xvortex's FTP v1.3
    Xvortex's Dumper v1.8
    Stooged's BackUp v2
    Stooged's App2Usb v1
    
PS4 Wi-Fi Settings (EASY):

    Network: PS4
    Password: qwertyuiop

"Test internet connection" also passes successfully with such settings!

Upload firmware in .bin format via NodeMCU-PyFlasher 3.0

CREDITS TO:

Al-Azif, Specter, Qwertyoruiopz, Flatz, XVortex, Stooged, LightningMods, Anonymous, Marcelstoer, The Open Orbis team, etc

---


**Прошивка для ESP8266**

Данный репозиторий содержит прошивку для модуля ESP8266 с поднятием вэб-сервера для хоста эксполитов/пэйлоадов Playstation 4 для ПО 5.05


Состав сборки (по мере выхода новых версий пэйлоады обновляются):

    MIRA+HEN
    Xvortex's HEN v1.6
    Xvortex's FTP v1.3
    Xvortex's Dumper v1.8
    Stooged's BackUp v2
    Stooged's App2Usb v1
    
Настройки PS4 Wi-Fi (метод - "Простой"):

    Network: PS4
    Password: qwertyuiop  

С данными настройками так же успешно проходится тест на подключение к интернету!

Прошивка предоставляется в формате bin для заливки в модуль с помощью NodeMCU-PyFlasher 3.0

Особая благодарность разработчикам:

Al-Azif, Specter, Qwertyoruiopz, Flatz, XVortex, Stooged, LightningMods, Anonymous, Marcelstoer, The Open Orbis team и т.д.
