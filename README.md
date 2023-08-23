# LaserCubeTD
Latest Laser Cube LAN / Wifi Python Script working for Touchdesigner 

**[VIDEO](https://www.youtube.com/watch?v=2ZKh2CRHdng)**

TouchDesigner is a node based programming environment for creative coding. This script provides support for the latests LaserCube connecting via Ethernet / Wifi for TouchDesigner.

Works on Windows 10 & 11 64 bit
Let met know about macOS? I've heard it works

## Prerequesites

1) Download and install **[TouchDesigner](https://derivative.ca/download)**
2) Download the latest release of this script **[HERE](https://github.com/NairoDorian/Laser-Cube-TouchDesigner/raw/main/TD_LASER_CUBE_WIFI_LAN_2022.toe)**
3) (Only if you want to connect to more than 1 Laser at the same time on a different network, each cube being in Server Mode) You need to change the IP assignated to the Cube by default, via Wifi & Ethernet

To setup the Cube address manualy, connect to it via Ethernet or Wifi and enter its configuration page, by default at http://192.168.1.1/
Default Username: LaserCubeUser
Default Password: Laser2020

By default in LAN & Wifi Server mode, the Cube will be at 192.168.1.1
For your 2nd cube in Server mode you should change the address for 192.168.2.1
If you have a third one in server mode, then it should be 192.168.3.1 and so on...


If you're using only 1 Laser cube the default settings are ok

One other setup could be to have 1 Cube in Server Mode and the other cubes in Client Mode and they should connect to the Server Cube.



## How To Laser

1) Boot your Laser cube and connect to it (You can go in  "Command Prompt" or "PowerShell" on Windows, and type "ipconfig" to check your IP Adress and the Cube address)
2) Open the TD_LASER_CUBE_WIFI_LAN.toe file
3) Click on the box called "TD_LASER_CUBE_WIFI_LAN" in its Parameters you should be able to change the LaserCube IP Address and the Sample Rate 30000 by default = 30kpps
4) Adjust the Intensity of the laser and the Scale to a lower value to be more careful thanks to the sliders on top and bottom of the ON / OFF button
5) Click on the ON / OFF Button to start sending data to the Laser Cube


## More Informations

Range of valid inputs are:
- X / Y: float between -1 and +1
- Red / Green / Blue: float between 0 and +1


Note that **[TDAsyncIO](https://github.com/sndmtk/TouchDesigner-asyncio)** is needed to run the script correctly in Touchdesigner, it's already included in the .toe
