# Digital-VLSI-SoC-design-and-planning
This repository contains materials from a 5-day workshop conducted by NASSCOM and VSD on SoC Design and Planning, It includes learning resources from VSD's instructional videos and lab work using the OpenLANE tool provided by NASSCOM.
# contents
# DAY 1-Inception of open-source EDA, OpenLANE and Sky130 PDK 
# DAY 2 -Good floorplan vs bad floorplan and introduction to library cells
# DAY 3 -Design library cell using Magic Layout and ngspice characterization
# DAY 4 -Pre-layout timing analysis and importance of good clock tree.
# DAY 5 -Final steps for RTL2GDS using tritonRoute and openSTA.
## DAY 1
### Inception of open-source EDA, OpenLANE and Sky130 PDK
#1-how-to-talk-to-computer">How to talk to computers
This is the Arduino Leonardo board, consisting of a Processor/SoC and various other interconnected devices and peripherals. The highlighted part in the above figure is the central block around which the entire VLSI design revolves.

The picture below depicts the layout of the entire microcontroller board.
<br>
![DAY1](https://github.com/user-attachments/assets/26e772f7-a089-46f3-b00c-b9aa2205d607)
<br>
Thus, this picture consists of various interconnect devices, external chips, and various other components. A few features of this layout are:
<ul>
  <li>The central part, the processor/SoC, is the layout of the chip highlighted on the Arduino board.</li>
  <li>It comprises various other devices like SRAM, EEPROM, ADCs, and other components that are combined and placed to make a microcontroller board.</li>
</ul>
<br>
Our main objective is to design a Processor/SoC, so the picture below depicts the design of a QFN-48 Package with the chip in the middle, connected by bond wires or interconnect wires.
<br>

![day1 2](https://github.com/user-attachments/assets/c21a2f5b-c6a8-423e-8de6-baa69abe142a)

<br>
This package also comprises a die, I/O pads, and a core. The layout of this is depicted below:
<br>
![day 1 3](https://github.com/user-attachments/assets/15f7f869-6341-4b90-a58a-7dd895d90499)
<br>
The core of this SoC consists of two major parts:
<ul>
  <li>**Foundry IPs:** These are the factories that help to implement the design on the silicon wafer and to make chips through their expertise. These chips made by the foundries are termed Foundry Intellectual Property.</li>
  <li>**Macros:** These are pure digital logic blocks.</li>
</ul>
<br>
![day1 4](https://github.com/user-attachments/assets/af929194-707e-4e2f-a885-5516c268c289)

<br>
We are using the RISC-V Architecture, also called Instruction Set Architecture (ISA), to design an SoC. The picture below depicts the flow from RTL to GDS.
<br>
![day1 6](https://github.com/user-attachments/assets/96ba8e2a-63cc-4974-92ee-23d30326b0bd)

<br>
Now, let's move on to how the software applications connect to the hardware. Shown below is the entire flow of how the software connects to the hardware.
<br>
![day1 7](https://github.com/user-attachments/assets/18ce15a5-8cff-4f75-bb00-1d035396a345)

<br>
We are taking the example of a stopwatch flow, and the implementation is done using RISC-V Architecture.
<br>
![day1 8](https://github.com/user-attachments/assets/13a42cae-c9e3-48f1-9664-9dd5508d36f3)

<br>
Deep diving into the flow, we observe that there is one more process after the assembler: the use of HDL (Hardware Description Language). We convert the binary code into HDL, which signifies the function that the entire hardware will perform with that bit stream. The next step after this is synthesizing the RTL flow for physical design implementation.
<br>
![day1 9](https://github.com/user-attachments/assets/328ce451-d75f-4b27-9863-61aeef24e132)

<br>
<hr>

#2-soc-design-and-openlane">SOC Design and OpenLANE
#3-get-familiar-to-open-source-eda-tools.


