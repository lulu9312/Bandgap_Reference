# Design of Simple Bandgap Reference circuit using Skywater 130 nm PDK

The purpose of this project is to implement the design of simple Bandgap Reference using Xschem and Ngspice which are  open source tools used for circuit design and simulation and Skywater 130 nm PDK (Process Design Kit)  

## Introduction

A Bandgap Reference is a circuit which gives constant voltage output (Vref) irrespective of temperature and supply variations. It is an important component of several analog and mixed signal IC’s.
Several circuits such as LDO,ADC,DAC ,Buck Converter, etc use Bandgap Reference as a building block.

## Description 

The main principle of Bandgap Reference is that the circuit is built with basic analogy of cancelling positive temperature coefficient which is PTAT and negative temperature coefficient which is CTAT that gives fixed voltage reference output independent of temperature and supply variations.
Basically we add two quantities with opposite temperature coefficient with proper weighting the resultanting sum quantity exhibits zero temperature coefficient.
The circuit contains four MOSFET's 2 upper PMOS for current mirroring and bottom NMOS are used to make voltage constant at points Vd and V2.The pnp transistor is used as diode in the circuit for CTAT and PTAT generation. The Vref is taken out from the third branch. The current is mirrored in the third brach with the help of PMOS. The volatge accross the resistor gives PTAT and voltage accross pnp transistor gives CTAT.

The circuit was designed using Xschem an open source schematic editor tool and  simulated using Ngspice an open source simulation tool. The circuit was simulated at TT corner and DC analysis was  performed over the temperature range of -40 to 125 (degree celcius). 

## Block Diagram 

![](Schematic%20%26%20Outputs/BGR_Block_Diagram.PNG)

## Schematic  

![](Schematic%20%26%20Outputs/BGR_Schematic.png) 

## Output Waveforms 

## Vref   

![](Schematic%20%26%20Outputs/BGR_Output.png) 

## CTAT 

![](Schematic%20%26%20Outputs/CTAT_Output.png) 

## PTAT 

![](Schematic%20%26%20Outputs/PTAT_Output.png) 

## Tools USed

1. Xschem  - Schematic Design 
2. Ngspice - Simulation
3. PDK - Skywater 130 nm PDK


## References

[1]  R. Akshaya and Siva Yellampalli  Analysis and design of Bandgap Reference (BGR) 

[2]  Youtube Videos - Analog Snippets

[3]  https://www.vlsisystemdesign.com/analog-bandgap-sky130/

## Author 

Pranav Dilip Lulu, Final Year B.Tech , E&TC , Vishwakarma Institute Of Information Technology , Pune.

Email: pranavlulu87@gmail.com


