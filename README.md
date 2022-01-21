# gerworks VR

Selbstgemachtes Vr-headset für \~100€ Tracking wird ermöglicht durch 1 Girosensor und optional 3 infrarot Leds Das Projekt basiert auf Relativty und Opentrack und benutzt ein abgeänderten Relativty Treiber

**!! Dieses Projekt ist ein Schulprojekt, kein Support !!**

## Support

Findest du das Projekt cool Supporte mich [ [hier](https://bunq.me/gerworks) ]

* [ ] 50 €
* [ ] 100 €
* [ ] 150 €

## Benötigte Teile

| Bauteil | Preis |    
|--|--|
| [Display](https://www.aliexpress.com/item/4000976201829.html) | 55,10 € |
| [LED](https://www.aliexpress.com/item/1005002655434560.html) | 0,77 € |
| [MPU-6050](https://www.aliexpress.com/item/32761922595.html) | 1,19 € |
| [Arduino](https://www.aliexpress.com/item/1005001706390728.html) | 4,33 € |
| [VR Headset](https://www.aliexpress.com/item/1005002549285047.html) | 41,32 € |
| [Driver Setup](https://bunq.me/gerworks) | 1 € (Bald Verfügbar) |


## Setup vom Arduino

Anschließen vom MPU-6050:

```
VCC     -> VCC  
GND     -> GND  
SDA(2) -> SDA  
SCL(3) -> SCL  
PIN 10  -> INT  
```

Danach kann die Firmware über die Arduino IDE übertragen werden Diese liegt in Firmware/[Firmware.ino](https://raw.githubusercontent.com/JannikBroer/gerworks-VR/main/firmware/firmware.ino) und in der Arduino IDE geh auf **Werkzeuge -> Boardinformarionen holen** und Notiere :

```
VID: 2341
PID: 8036
```

Diese Informationen sind in Hexadezimal angegeben, wir benötigen die aber als Dezimal Dies kannst du auf dieser Seite machen [ [hier](https://www.rapidtables.com/convert/number/hex-to-decimal.html) ]

## Setup SteamVR

***!!Hierfür brauchst du den Treiber aus der Bestelliste!!***

![](https://raw.githubusercontent.com/JannikBroer/gerworks-VR/main/doku_extras/Driver-Beschriftet.PNG)

Starte driver.exe trage deine Dezimal *VID* und *PID* info in die vorgesehenen Felder ein wähle die Auflösung deines Hauptbildschirmes und klicke auf speichern 

## Fertig

Starte in Steam -> SteamVR Vr-headset Fertig eingerichtet!
