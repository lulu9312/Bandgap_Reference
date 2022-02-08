# Design of simple Bandgap Reference circuit using Skywater 130 nm PDK

The purpose of this project is to implement the design of simple Bandgap Reference using Xschem ,Ngspice which are  open source tools used for circuit design and simulation and Skywater 130 nm PDK (Process Design Kit)  
## Introduction
A Bandgap Reference is a circuit which gives constant voltage output (Vref) irrespective of temperature and supply variations. It is an important component of several analog and mixed signal IC’s.
Several circuits such as LDO,ADC,DAC ,Buck Converter, etc use Bandgap Reference as a building block.

## Description 
The main principle of Bandgap Reference is that the circuit is built with basic analogy of cancelling positive temperature coefficient which is PTAT and negative temperature coefficient which is CTAT that gives fixed voltage reference output independent of temperature and supply variations.
Basically we add two quantities with opposite temperature coefficient with proper weighting the resultanting sum quantity exhibits zero temperature coefficient.

## Block Diagram 
![Screenshot](BGR_Block_Diagram.PNG)

