ECE281_Lab4
===========
#Design
ALU Design
----------

To implement the various actions for which the ALU is responsible, in-line commands that take advantage of the inherent features of vhdl were used, using one case statement for each function of the ALU.  The largest issue that was encontered was understanding that both the LDA command and IN command came straight from the Data Bus.  The simulation for the ALU is below:

![](https://github.com/C16erikthompson/ECE281_Lab4/blob/master/ALU_Waveform.png?raw=true)

Upon manual inspection of the Waveform, I found that each command worked as expected.

Datapath
---------

Designing the Datapath relied heavily upon the diagram of the PRISM architecture provided in the PRISM manual.  Being given the basic form of a register with the provided program counter, I looked at the inputs and outputs for each register and defined their interactions in a manner similar to that in the program counter.  The only difficulty during the design process lie in the creation of the address selector register, which required the concatenation of the MARHi and MARLo register outputs.  There were no major alterations made to the character of the Datapath in our VHDL programming.  The Waveform for the Datapath is displayed below:

![](https://github.com/C16erikthompson/ECE281_Lab4/blob/master/Datapath_Waveform.png?raw=true)

To initially verify that the waveform was performing corectly, I simply compared its output to that provided in Lab 4.  A more in-depth aalysis of the waveform output follows.

#Reverse Engineering




