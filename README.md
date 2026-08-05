Power Blink  ;)
---
Power blink is a power bank–type PCB module, mainly designed to charge batteries safely :B  

it has a screen that tells you about the charge  
o m g 

<img width="1917" height="1198" alt="Captura de pantalla 2026-07-30 190109" src="https://github.com/user-attachments/assets/3b539512-09d2-47b9-9140-d1e108273b01" />
<img width="1917" height="1198" alt="Captura de pantalla 2026-07-30 190210" src="https://github.com/user-attachments/assets/fedccf86-5838-4aba-89ed-204fc9c0ff5c" />
<img width="1917" height="1198" alt="Captura de pantalla 2026-07-30 190120" src="https://github.com/user-attachments/assets/536a18ba-14db-4731-8c40-745f2834834a" />


BTW BTW BTW low key look at my [JOURNAL.MD WOOWOWOWOWOWWOWOOOO!]([https://github.com/annaastrs-svg/PCB-Power-Blink/blob/actualizacion/journal.md](https://github.com/annaastrs-svg/PCB-Power-Blink/blob/main/Journal.md))

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

| Component | Purpose | Qty | Price | link|
|---|---|---|---|---|
| LiPo Battery 3.7V | Fuente de energía principal | 1 | ~$2.29 | i alrdy have one lolazo |
| TP4056-42-ESOP8 | IC de carga | 1 | ~$0.09 | [LCSC C16581](https://www.lcsc.com/product-detail/Battery-Management-ICs_TOPPOWER-Nanjing-Extension-Microelectronics-TP4056-42-ESOP8_C16581.html) |
| DW01A-G | Controlador de protección | 1 | ~$0.07 | [LCSC C61503](https://www.lcsc.com/product-detail/C61503.html) |
| FS8205A | MOSFETs de protección | 1 | ~$0.03 | [LCSC C908265](https://www.lcsc.com/product-detail/MOSFETs_FUXINSEMI-FS8205A_C908265.html) |
| MAX17048G+T10 | Fuel gauge (I2C) | 1 | ~$1.34 | [LCSC C2682616](https://www.lcsc.com/product-detail/C2682616.html) |
| ATtiny1614-SSN | Microcontrolador | 1 | ~$1.67 | [LCSC C614832](https://www.lcsc.com/product-detail/Microcontroller-Units-MCUs-MPUs-SOCs_Microchip-Tech-ATTINY1614-SSN_C614832.html) |
| MT3608 | Boost converter a 5V | 1 | ~$0.11 | [LCSC C84817](https://www.lcsc.com/product-detail/C84817.html) |
| USB-C Receptacle (Hroparts) | Entrada de carga | 1 | ~$0.10 | [LCSC C165948](https://www.lcsc.com/product-detail/C165948.html) |
| USB-A Receptacle THT | Salida de energía | 1 | ~$0.15 | genérico, cualquier tienda |
| OLED 0.91" I2C SSD1306 | Pantalla de batería | 1 | ~$1.20 | [AliExpress](https://www.aliexpress.com/item/33024849277.html) |
| Pulsador momentáneo 6mm | Despertar pantalla | 1 | ~$0.05 | genérico |
| SS34 Schottky | Diodo del boost | 1 | ~$0.05 | genérico |
| LEDs indicadores (CHRG/STDBY) | Indicadores de carga | 2 | ~$0.02 ea. | genérico |
| Resistencias SMD (varias) | 5.1k, 4.7k, 2.4k, 470, 1k, 10k, 75k | 10 | ~$0.01 ea. | genérico |
| Capacitores SMD (10-22µF) | Desacople/filtro | 6 | ~$0.03 ea. | genérico |

**Estimated Total: ~$8.00 USD (sin batería yey )**

## Connection table

| Componente | Pin | → | Componente | Pin |
|---|---|---|---|---|
| J3 (USB-C) | VBUS | → | U8 (TP4056) | VCC |
| J3 (USB-C) | CC1, CC2 | → | GND | (vía R1, R2 5.1k) |
| U8 (TP4056) | CE | → | VCC | |
| U8 (TP4056) | CHRG | → | LED D2 | → VCC |
| U8 (TP4056) | STDBY | → | LED D1 | → VCC |
| U8 (TP4056) | PROG | → | GND | (vía 2.4k) |
| U8 (TP4056) | BAT | → | +BATT (raw) | |
| Batería | + | → | Q1 (FS8205A) | S1 |
| Batería | − | → | GND | |
| Q1 (FS8205A) | S2 | → | −BATT | |
| Q1 (FS8205A) | G1 | → | U3 (DW01A) | OD |
| Q1 (FS8205A) | D1/D2 | → | U3 (DW01A) | CS (vía R6 1k) |
| Q1 (FS8205A) | G2 | → | U3 (DW01A) | OC |
| U3 (DW01A) | VCC | → | +BATT | (vía R5 470) |
| U3 (DW01A) | GND | → | −BATT | |
| U4 (MAX17048) | VDD | → | +BATT | |
| U4 (MAX17048) | GND | → | GND | |
| U4 (MAX17048) | SDA, SCL | → | Bus I2C | (compartido con U5, U6) |
| U5 (ATtiny1614) | VDD | → | +BATT | |
| U5 (ATtiny1614) | GND | → | GND | |
| U5 (ATtiny1614) | PA1 | → | Bus I2C | SDA |
| U5 (ATtiny1614) | PA2 | → | Bus I2C | SCL |
| U5 (ATtiny1614) | PA3 | → | SW1 | (botón) |
| U5 (ATtiny1614) | PA0/UPDI | → | J2 | Header de programación |
| Bus I2C | SDA, SCL | → | GND | (vía R9, R10 4.7k a +BATT) |
| U6 (OLED) | VCC | → | +BATT | |
| U6 (OLED) | GND | → | GND | |
| U6 (OLED) | SDA, SCL | → | Bus I2C | |
| U1 (MT3608) | IN | → | +BATT | |
| U1 (MT3608) | GND | → | GND | |
| U1 (MT3608) | SW | → | L1, D3 | → VOUT |
| U1 (MT3608) | FB | → | R7 (10k)/R8 (75k) | divisor |
| U1 (MT3608) | EN | → | +BATT | |
| J1 (USB-A) | VBUS | → | VOUT | |
| J1 (USB-A) | D+, D− | → | (puenteados entre sí) | |
| J1 (USB-A) | GND | → | GND | |



TUTORIAL & HOW DOES ITR WORK? HUH 
--

Open the Power Blinck file, the schematic, and the PCB in KiCad.
The symbols and footprints of the components are not included by default in KiCAS, but I attached the footprints and symbols in the PCB files. 
Add them as a library before opening the project, run the ERC and DRC to make sure everything is clean. 
To manufacture, use the Gerber files; they can be uploaded directly to PCBWay and like that :B


The circuit is divided into 4 blocks. The input and charging part is the USB-C, which receives the charge, and the TP4056, which safely charges the battery. 
The battery and protection section, with the DW01A and FS8205A, protects the cell against overcharge, overdischarge, and short circuits. 
The monitoring is done by the MAX17048, which measures the battery percentage, and the ARINY1614, which displays it on the OLED screen.
The power output is the MT3608, which boosts the battery voltage to a stable 5V for the USB-A port.


PCB WAY 
--
chat is this fire? 
<img width="1892" height="1080" alt="Captura de pantalla 2026-07-30 205220" src="https://github.com/user-attachments/assets/95d51506-b5a2-4af4-818e-9471622a5fa3" />
<img width="887" height="237" alt="Captura de pantalla 2026-07-30 205137" src="https://github.com/user-attachments/assets/9d6b85a6-1869-4088-8949-2795df3cac88" />


w o w  isnt it pretty :O 


NOTES
---
This project was made for [MACONDO](https://macondo.hackclub.com/dashboard)

ill improve this project, there some things that ill change, maybe chips, modules or somthing like that. if u want to do this lil tutorial dont get mad at me if it doesnt work lolazo 
