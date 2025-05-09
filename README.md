# OPEnS_LTE

Wiki: [LTE](https://github.com/OPEnSLab-OSU/OPEnS-Lab-Home/wiki/LTE)

An LTE module based on the Ublox SARA-R410M series chipset for IoT and remote sensing applications. 

<p align="center">
 <img src="https://github.com/user-attachments/assets/250219a9-78e0-4130-b314-0bae8dfcf8aa" width="80%">
 
</p>

**<div align="center">Three dimensional rendering of "OPEnS LTE" in Autodesk Fusion 360</div>**

"OPEnS LTE" measures 60mm x 26mm (Length x Width, rounded up to nearest integer). 

## Documentation Sections: 
1) Breakdown of Repository Contents.
2) Instructions for Using "OPEnS LTE."
3) Technical Documentation (Specifications, Schematics, Simulation Files, etc.).
4) How to Procure "OPEnS LTE."

### Breakdown of Repository Contents:
1) "BOM for PCBWay.xlsx" --> Bill of materials (BOM) file (for upload to PCBWay's assembly service).
2) "Gerber.zip" --> PCB manufacturing files (for upload to PCBWay's assembly service).
3) "OPEnS LTE - REV 1.f3z" --> Design files archive (open using Autodesk Fusion).
4) "PnP.xlsx" --> Pick and place centroid file (for upload to PCBWay's assembly service).
5) "README.md" --> Repository readme file.

<hr>
<p align="center">
 <img  src="https://github.com/user-attachments/assets/a4a6ea44-4d34-4dec-822b-46256c4834db" width="45%">   
 <img src="https://github.com/user-attachments/assets/212ad254-31b0-47d6-9b96-c7cdee6eeeef" width="45%">
</p>
<div align="center">Functional prototype of "OPEnS LTE" (left), "OPEnS LTE" prototype connected to the internet (right) </div>
<hr>

### Instructions for Using "OPEnS LTE:"

### Technical Documentation:

#### Pin Function:
- VCC - Module power supply for SARA-R410M and other onboard components.
- REF - Reference logic level for external microprocessor (supports 3.3V-5V logic).
- PWR - Pin to wakeup SARA-R410M.
- RST - Pin to reset SARA-R410M.
- TX - UART data out to microprocessor.
- RX - UART data in from microprocessor.

#### Specification Tables:

##### Recommended Operating Voltages:
| Pin | Mininum (V) | Typical (V) | Maximum (V) |
|-----|-------------|-------------|-------------|
| VCC | 3.2 | 3.8 | 4.2 | 
| REF | 1.8 | VCC | 5.5 |
| PWR | GND | GND | VCC |
| RST | GND | GND | VCC |
| TX | GND | ~ | REF
| RX | GND | ~ | REF

##### Absolute Voltage Limits:
| Pin | Mininum (V) | Maximum (V) |
|-----|-------------|-------------|
| VCC | -0.5 | 5.2 |
| REF | -0.5 | 6.5 |
| PWR | -18 | 18 |
| RST | -18 | 18 |
| TX | -0.5 | REF+0.5 |
| RX | -0.5 | REF+0.5 |

#### Schematic diagram for "OPEnS LTE:"
![image](https://github.com/user-attachments/assets/b830ba85-dc76-46fc-bde1-5ae7f1cbade6)



