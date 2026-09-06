# Custom ESP32-S3 Board

This repository contains the schematic and PCB design files for a custom ESP32-S3 development board featuring dual USB-C connectors and an onboard FTDI UART bridge. 

## Board Specifications

This board was designed in Altium Designer utilizing a 4-layer stackup (Signal - Power - GND - Signal). Using inner layers as dedicated solid planes for Power and Ground minimizes electromagnetic interference (EMI), provides a clean return path for high-speed signals, and ensures stable power distribution across the board. The design features a dual USB-C interface: one port is connected via an onboard FTDI chip for reliable UART programming and serial debugging, while the other is routed directly to the ESP32's native USB pins to utilize internal USB capabilities.

## 3D View and Schematic
<img width="1351" height="613" alt="3d" src="https://github.com/user-attachments/assets/512cc94d-e631-4606-94cd-e96ad43d31e4" />
<img width="1048" height="592" alt="3d_1" src="https://github.com/user-attachments/assets/f7fc507d-9a69-45d9-8c40-0f7fcd67c97a" />
<img width="1293" height="631" alt="3d_back" src="https://github.com/user-attachments/assets/3673538f-85be-47e4-8a2d-796679168755" />
<img width="3509" height="2481" alt="schematic" src="https://github.com/user-attachments/assets/e1c77435-a21b-4359-87c3-10362c437575" />


## PCB Layers
<img width="1308" height="673" alt="l" src="https://github.com/user-attachments/assets/8ea5e16f-ed72-46f1-a98f-dce63ec759cd" />
<img width="1371" height="615" alt="l1" src="https://github.com/user-attachments/assets/cff79014-4bd6-4fae-8bc6-8d1512326d8d" />
<img width="1613" height="686" alt="l2" src="https://github.com/user-attachments/assets/241b25a1-c385-4b2d-9586-40795589452c" />
<img width="1538" height="651" alt="l3" src="https://github.com/user-attachments/assets/c0cedf14-5050-48bb-b4f2-ea5f37d945b3" />
<img width="1546" height="662" alt="l4" src="https://github.com/user-attachments/assets/7e573946-cdb6-40f9-8d95-b93181e23d2e" />


## Bill of Materials 

| Designator | Component | Description |
| :--- | :--- | :--- |
| **MOD1** | ESP32-S3-MINI-1 | Wi-Fi and Bluetooth LE MCU Module |
| **U1** | FT232RNL | USB to UART Interface |
| **REG1** | AZ1117CH-3.3 | 3.3V Linear Voltage Regulator (LDO) |
| **USBC1, USBC2**| TYPE-C-31-M-12 | 16-pin USB Type-C Receptacle |
| **Q1, Q2** | S8050 | NPN Transistors (Auto-reset circuit) |
| **BTN1, BTN2** | Tactile Switch | Boot / User and Reset Buttons |

Special thanks to Robert Feranec for his guidance 
