# gerworks-VR
### Vr for 100€
Open Source VR Headset
This Projekt is based on Relativty
and Opentrack

Products used with this config:
[Arduino Micro](https://www.aliexpress.com/item/1005001706390728.html) , [Girosensot](https://www.aliexpress.com/item/32761922595.html) , [Infrared LED](https://www.aliexpress.com/item/1005002655434560.html) , [Display](https://www.aliexpress.com/item/32884621131.html) , [Case](https://www.aliexpress.com/item/1005002549285047.html) = 88,33€
Traking is achived trough Girsosensor and Infared LED (you need 3 tracking Points)



### Arduino Setup

Arduino Pinout to MPU-6050:
```
5V      -> VCC  
GND     -> GND  
SDA(20) -> SDA  
SCL(21) -> SCL  
PIN 2   -> INT  
```
now you can install the firmware.ino

### Steam Setup

1. Install [SteamVR](https://store.steampowered.com/app/250820/SteamVR/).
2. Copy the gerworksvr driver to "...\Steam\steamapps\common\SteamVR\drivers"
