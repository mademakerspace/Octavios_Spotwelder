# Octavio's Spot welder

![alt text](https://github.com/mademakerspace/Octavios_Spotwelder/blob/master/img/IMG_20170319_160101.jpg "Awesomeness!")

## Introduction:
Nowadays it is very common to use batteries on makers projects. The propose of the project is to be able to solder easily on lithium batteries without using battery case holders. This cool solution allows to build a small and cheap spot welding machine.

Spot welders based on capacitors use large capacitors to store electrical energy and release it quickly. Capacitors can deliver large current peaks extremely fast. The capacitors discharge energy is dissipated due to the metal resistance in the form of heat which melts and fuses metal pieces. A large current passes through the work piece and weld nugget is formed in few milliseconds.

Most part of the energy goes into weld formation and less part into heating the surrounding material. This is also important because the properties of the metal would have changed from rapid heating and cooling. These changes are localized in the small area around the weld spot.

Capacitive resistance welders have many advantages:
• Very short process time
• No consumables, such as brazing materials, solder, or welding rods
• Operator safety because of low voltage
• Clean and environmentally friendly
• A reliable electro-mechanical joint is formed

## List of material:
* 6x Ultra capacitor 2,7V 500F  (22€)
* Arduino nano (1.6€)
* RGB Led (generic)
* 48 Mosfet (2,8 €)
* 1 BUZ10 mosfet (1€)
* DCDC (5€)
* Battery (2€)
* **TOTAL: ~34€**

Schematic and code:
Code and schematic can be found here: [**Schematic**](https://github.com/mademakerspace/Octavios_Spotwelder/blob/master/Schematic.png)

Red wires on schematic should have big sections as you can see on the post images. Mosfet arrays are mounted on a custom-made PCB.

![](https://github.com/mademakerspace/Octavios_Spotwelder/blob/master/img/IMG_20170319_160244.jpg)

When arduino is power up setup() routine checks battery and capacitors state of charge. Different led colors are used to indicate state of charge SOC (blue > green > yellow > red).

After setup, arduino checks if both electrodes are short-circuited for more than a second (it means peaces are ready and discharge can be done).

## Credits:
Design: Octavio
Support: Xavier Giménez

## References:

http://www.amadamiyachi.com/servlet/servlet.FileDownload?retURL=%2Fapex%2Feducationalresources_articles&file=01530000000Jybm

http://www.powerstream.com/ss/PSSunstoneSPWelderIP.pdf

http://www.batteryspace.com/prod-specs/5997.htm

Other projects:

http://www.instructables.com/id/Dual-Pulse-Capacitive-Discharge-Spot-Welder/?ALLSTEPS
