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


In case you are using a different board, the process to get the right values is as below:

1.	Plug your board in

2.	Select your board in Arduino IDE and click Tools/Get Board info. you will see something like this:

```
	BN: Arduino Due (Native USB Port)
	VID: 2341
	PID: 003e
	SN: HIDHB
```
3.	Make note of the VID and PID numbers. These are hexadecimal values.

	To apply them to the config, they need to be converted to int.
	
	If you are unsure how to do that, there is plenty online converters available.
	
	Such as: https://www.rapidtables.com/convert/number/hex-to-decimal.html

4.	Change your hmdPid and hmdVid values to the converted values.

### Steam Setup

1. Install [SteamVR](https://store.steampowered.com/app/250820/SteamVR/).
2. Copy the gerworksvr driver to "...\Steam\steamapps\common\SteamVR\drivers"

### Opentrack 

1.Start Opentrack choose your tracking method (in this case PointTracker 1.1) and click on the litle hamer icon and configure it.
</br>
2.Set Output to freetrack 2.0 Enhanced and under Filter leave it blank, now click on START 
</br>
3. THATS IT 
