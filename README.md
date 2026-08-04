Power Blink  ;)
---
Power blink is a power bank–type PCB module, mainly designed to charge batteries safely :B  
it has a screen that tells you about the charge  
o m g 

<img width="1917" height="1198" alt="Captura de pantalla 2026-07-30 190109" src="https://github.com/user-attachments/assets/3b539512-09d2-47b9-9140-d1e108273b01" />
<img width="1917" height="1198" alt="Captura de pantalla 2026-07-30 190210" src="https://github.com/user-attachments/assets/fedccf86-5838-4aba-89ed-204fc9c0ff5c" />
<img width="1917" height="1198" alt="Captura de pantalla 2026-07-30 190120" src="https://github.com/user-attachments/assets/536a18ba-14db-4731-8c40-745f2834834a" />


BTW BTW BTW low key look at my [JOURNAL.MD WOOWOWOWOWOWWOWOOOO!](https://github.com/annaastrs-svg/PCB-Power-Blink/blob/actualizacion/journal.md)

KiCAD
--
Esquematico
<img width="1917" height="1198" alt="Captura de pantalla 2026-07-30 190951" src="https://github.com/user-attachments/assets/afa194a7-7679-4854-be93-d494e4615f40" />

PCB
<img width="1917" height="1198" alt="Captura de pantalla 2026-07-30 190232" src="https://github.com/user-attachments/assets/de16b25a-2efa-479f-aa51-31d7f36ac493" />

3D VIEW 🔥
<img width="1907" height="1190" alt="Captura de pantalla 2026-07-30 190155" src="https://github.com/user-attachments/assets/977e1058-8c3f-4128-96f4-4f5f3c1b6df2" />

PCB Huellas 
---
<img width="907" height="627" alt="Captura de pantalla 2026-07-30 190930" src="https://github.com/user-attachments/assets/6afcf197-b94e-4510-94de-9e18b1202585" />


Tabla de Conexiones
---



CAD
---
 CAD detailes :
 The PCB is 55.8067 mm long & 40.9582 tall so i added 2 mm in all sides so it can fit in 
 the button is 6x6 mm
 the oled is 5.584 & 22.384 long
 the entry of c 14.4 long 
 the entry of a is 8.94 cm long 
 <img width="427" height="320" alt="image" src="https://github.com/user-attachments/assets/090b6b10-d9fa-4980-a083-6240affb0ce4" />


<img width="1055" height="658" alt="Captura de pantalla 2026-08-04 135139" src="https://github.com/user-attachments/assets/16225cec-28f6-403d-8fbd-47161a59f7aa" />
<img width="1147" height="742" alt="Captura de pantalla 2026-08-04 135057" src="https://github.com/user-attachments/assets/ee97f995-f0a4-42c5-8fcf-506cbf82f365" />
<img width="692" height="392" alt="Captura de pantalla 2026-08-04 135509" src="https://github.com/user-attachments/assets/6f5ab02c-db72-4bd9-8e2e-df1c571dbaae" />

[look CAD file ](https://github.com/annaastrs-svg/PCB-Power-Blink/tree/main/CAD)

BOM 
---
[BOM file ](https://github.com/annaastrs-svg/Battle-Bot-/blob/actualizacion/laminax_bot.ino)


PCB WAY 
chat is this fire? 
<img width="1892" height="1080" alt="Captura de pantalla 2026-07-30 205220" src="https://github.com/user-attachments/assets/95d51506-b5a2-4af4-818e-9471622a5fa3" />
<img width="887" height="237" alt="Captura de pantalla 2026-07-30 205137" src="https://github.com/user-attachments/assets/9d6b85a6-1869-4088-8949-2795df3cac88" />
w o w  isnt it pretty :O 



TUTORIAL & HOW DOES ITR WORK? HUH 
--
The circuit is divided into 4 blocks. The input and charging part is the USB-C, which receives the charge, and the TP4056, which safely charges the battery. The battery and protection section, with the DW01A and FS8205A, protects the cell against overcharge, overdischarge, and short circuits. The monitoring is done by the MAX17048, which measures the battery percentage, and the ARINY1614, which displays it on the OLED screen. The power output is the MT3608, which boosts the battery voltage to a stable 5V for the USB-A port.
Open the Power Blinck file, the schematic, and the PCB in KiCad. The symbols and footprints of the components are not included by default in KiCAS, but I attached the footprints and symbols in the PCB files. Add them as a library before opening the project, run the ERC and DRC to make sure everything is clean. To manufacture, use the Gerber files; they can be uploaded directly to PCBWay and like that :B


NOTES
---
This project was made for [MACONDO](https://macondo.hackclub.com/dashboard)

ill improve this project, there some things that ill change, maybe chips, modules or somthing like that. if u want to do this lil tutorial dont get mad at me if it doesnt work lolazo 
