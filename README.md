Power Blink  ;)
---
A power bank PCB Module designed in KiCAD, to safly charge lithium battery and u can look in the display the battery percentage on the oled screen
o m g 

<img width="810" height="260" alt="Captura de pantalla 2026-08-05 142008" src="https://github.com/user-attachments/assets/0b0579c5-1176-459f-88b6-b029ab9737bf" />
<img width="1260" height="820" alt="Captura de pantalla 2026-08-05 142235" src="https://github.com/user-attachments/assets/e569520b-4762-46c5-a0c4-9efae5061a60" />


Power blink charges though USB-C and delivers power though USB-A, with an onboard fuel gauge and microcontroller driving a small OLED display that shows the actuall battery charge level :B 

BTW BTW BTW low key look at my [JOURNAL.MD WOOWOWOWOWOWWOWOOOO!](https://github.com/annaastrs-svg/PCB-Power-Blink/blob/main/Journal.md)

KiCAD
--
Esquematico
--
<img width="1080" height="652" alt="Captura de pantalla 2026-08-05 123812" src="https://github.com/user-attachments/assets/4a7ed007-5ebb-4c73-bd94-06cb2228b655" />


PCB
--
<img width="1403" height="1045" alt="Captura de pantalla 2026-08-05 142304" src="https://github.com/user-attachments/assets/c2235250-6471-4326-9b0b-aec46ba79d01" />

3D VIEW 
--
<img width="1278" height="927" alt="Captura de pantalla 2026-08-05 142138" src="https://github.com/user-attachments/assets/54519417-d647-4133-a2bf-63268562e42b" />


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
 
 (btw ignore the pcb it was a scratch )
 <img width="427" height="320" alt="image" src="https://github.com/user-attachments/assets/090b6b10-d9fa-4980-a083-6240affb0ce4" />


<img width="1055" height="658" alt="Captura de pantalla 2026-08-04 135139" src="https://github.com/user-attachments/assets/16225cec-28f6-403d-8fbd-47161a59f7aa" />
<img width="1147" height="742" alt="Captura de pantalla 2026-08-04 135057" src="https://github.com/user-attachments/assets/ee97f995-f0a4-42c5-8fcf-506cbf82f365" />

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


The circuit is divided into 4 blocks. The input and charging part is the USB-C, which receives the charge, and the TP4056, which safely charges the battery. (TP4056 SAFE)

The battery and protection section, with the DW01A and FS8205A, protects the cell against overcharge, overdischarge, and short circuits. (DW01A , FS8205A PROTECTS )

The monitoring is done by the MAX17048, which measures the battery percentage, and the ARINY1614, which displays it on the OLED screen. (MAX17048 MEASURE , ARINY1614 READS AND SHOW  )

The power output is the MT3608, which boosts the battery voltage to a stable 5V for the USB-A port. (MT3608 STABLE VOLTAGES)

i loved making this pcb cus it looks easy but at the moment u see a lot of chips/modules with a lot of pins u cant avoid panic
in my projects i struggle a lot with power distribution and this had helpped me a lot :B 

PCB WAY 
--
THIS IS THE V.1 OF THE PROJECT !! (I did it 2 times cus i didnt like v.1)

<img width="887" height="237" alt="Captura de pantalla 2026-07-30 205137" src="https://github.com/user-attachments/assets/9d6b85a6-1869-4088-8949-2795df3cac88" />

This is V.2 in PCB basics simulation of the pcb :B 

<img width="810" height="260" alt="image" src="https://github.com/user-attachments/assets/2fe53eb1-610c-49d5-94a6-7ce7c6ea0007" />



NOTES
---
This project was made for [MACONDO](https://macondo.hackclub.com/dashboard)

ill improve this project, there some things that ill change, maybe chips, modules or somthing like that. if u want to do this lil tutorial dont get mad at me if it doesnt work lolazo, Im 80 % sure it works !! 

