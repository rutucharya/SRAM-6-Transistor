# SRAM 6-Transistor

# Introduction
6T static random-access memory is a type of semiconductor memory that uses bistable latching circuitry to store each bit. The term static differentiates it from dynamic RAM which must be periodically refreshed. This report demonstrates the design of a 6 - Transistor Static RAM cell that stores 1bit of data and also explains its READ and WRITE operation, implementation of design, and explains the function of how it stores 1bit in a cell.


# Circuit Details
SRAM, known as Static Random Access Memory also known as Read Write Memory has become a very crucial part of SOCs and ASIC. As the basic unit of SRAM is the SRAM cell, the need of SRAM cell is to perform stable and robust read/write operation in such a way that it consumes the least power and enhance the on-chip storage capacity. The given circuit demonstrates six transistor SRAM cell, out of which four transistors Q1, Q2, Q3, and Q4 forms a cross-coupled CMOS inverter, that itself becomes a memory. And remaining two nmos act as access transistors. These access transistors are connected to the bit line and bit line bar that are denoted by “BL & BLB”. And word line here denoted by “WL” is connected to access transistors when the word line is set on, the access transistors can be accessed and similarly when a word line is set off the content of the memory comes set to hold state as the access transistors are turned off, and as a result, the data will remain unchanged in the cell, for the write operation bit line and bit line bar acts as input lines and for reading operation these lines would act as output lines. We would design this circuit using open-source SkyWater 130nm PDKs.


# Schematic
![sch](https://user-images.githubusercontent.com/98079644/194717104-327ede7e-6b35-48ae-a51c-95abadcc042e.png)


# Inverter Verilog Code
![veri](https://user-images.githubusercontent.com/98079644/194717160-cbb51251-d8b7-46d3-907b-4e359e7f5cf8.png)


# Voltage Source and Pulses applied as input signals
![ss](https://user-images.githubusercontent.com/98079644/194717226-3c423b7c-d530-4292-90d8-16173ab1e92e.png)


# Waveform for Write operation
![write1](https://user-images.githubusercontent.com/98079644/194719972-f937c3c4-48a4-402f-bd50-5dd27edcd2d9.png)


# Waveform for Read operation
![read1](https://user-images.githubusercontent.com/98079644/194719980-194b09ae-01b7-4720-9224-a856ca5a6dd1.png)


# ZIP Files
[SRAM.zip](https://github.com/rutucharya/SRAM-6-Transistor-/files/9739767/SRAM.zip)


# Acknowledgement
http://iitb.ac.in/
https://www.google.co.in/
https://fossee.in/
https://spoken-tutorial.org/
https://www.vlsisystemdesign.com/
https://www.c2s.gov.in/


# Reference
https://www.iosrjournals.org/iosr-jvlsi.html?ref=https://githubhelp.com
