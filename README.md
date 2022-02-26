# Design a 2-bit magnitude comparator using 28nm CMOS Technology

The design of a 2-bit magnitude comparator utilizing Synopsys Custom Compiler on 28nm CMOS technology is shown in this repository.

##  Table of Content
   * [Abstract](#Abstract)
   * [Introduction](#Introduction)
   * [Detailed Explanation](#Detailed-Explanation)
   * [Apparatus](#Apparatus)
   * [CMOS NOT Gate](#CMOS-NOT-Gate)
   * [CMOS 2 Input AND Gate](#CMOS-2-Input-AND-Gate)
   * [CMOS 3 Input AND Gate](#CMOS-3-Input-AND-Gate)
   * [CMOS 3 Input OR Gate](#CMOS-3-Input-OR-Gate)
   * [CMOS XNOR Gate](#CMOS-XNOR-Gate)
   * [2-Bit magnitude comparator Module](#2-Bit-magnitude-comparator-Module)
   * [Simulations](#Simulations)
   * [Netlist](#Netlist)
   * [Acknowledgements](#Acknowledgements)
   * [References](#References)
 




##  Abstract
This study offers a CMOS circuit for a 2-bit magnitude comparator. The most fundamental arithmetic operation is comparison, which determines whether one number is greater   than, equal to, or less than another. The most basic component that conducts comparison operations is the comparator. In addition, we will use the Synopsys tool to simulate a 2-bit magnitude comparator that is implemented in 28nm technology.
	

##  Introduction
In digital system, comparison of two numbers is an arithmetic operation that determines if one number is greater than, equal to, or less than the other number [1]. A comparator is a logic circuit used to compare the magnitude of two binary numbers. Depending on the design, it may either simply provide an output that is active (goes HIGH) when the two numbers are equal, or additionally provide outputs that signify which of the numbers is greater when equality does not hold


##  Construction and working of 2-bit magnitude comparator
2-Bit Magnitude Comparator Compares two numbers each having two bits (A1, A0 & B1, B0). The logic for a 2-bit numbers be A=A1A0 and B=B1B0. Two binary numbers are equal, if and only if all their corresponding bits coincide. 


![image](https://user-images.githubusercontent.com/71437573/155836169-18677b92-1f64-4f75-8d88-c36b03ed9ff8.png)

  Figure 01: 2-bit Magnitude Comparator
  
The outcome of comparison is specified by three binary variables that indicate whether A>B, A=B, or A<B[1].

> Truth Table

   ![image](https://user-images.githubusercontent.com/71437573/155836295-09a2be60-15aa-42e3-bcb1-dfb780098474.png)

> KARNAUGH MAPPING

The Karnaugh map (K-map) method, is a systematic method to simplifying the Boolean expression.

1. For A>B

    ![image](https://user-images.githubusercontent.com/71437573/155836397-e808e052-58fe-4ebb-94c5-87bab51e14f3.png)

    A>B: A1B1’ + A0B1’B0’ + A1A0B0’


2. For A=B

    ![image](https://user-images.githubusercontent.com/71437573/155836420-bc449b9f-1362-44b5-b524-dcfd516334b8.png)
 
    A=B: A1’A0’B1’B0’ + A1’A0B1’B0 + A1A0B1B0 + A1A0’B1B0’
    
       : A1’B1’ (A0’B0’ + A0B0) + A1B1 (A0B0 + A0’B0’)
       : (A0B0 + A0’B0’) (A1B1 + A1’B1’)
       : (A0 Ex-Nor B0) (A1 Ex-Nor B1)

3. For A<B
	   
     ![image](https://user-images.githubusercontent.com/71437573/155836498-ad9e1d93-4b16-4e7d-a64e-7854c6d5ebec.png)
	   
     A<B: A1’B1 + A0’B1B0 + A1’A0’B0

> CIRCUIT DAIGRAM

   ![image](https://user-images.githubusercontent.com/71437573/155836911-c44ee1b6-1162-4362-a4ec-e598086991d0.png)
   
   Figure 02: Circuit Diagram of 2-bit magnitude comparator

##  Apparatus

- Synopsys Custom CompilerTM is a cutting-edge design environment for full-custom analogue, custom digital, and mixed-signal ICs. Custom Compiler, the brains behind the Synopsys Custom Design Platform, lets you enter designs, control simulations, and change custom layouts. It provides industry-leading productivity, performance, and ease-of-use while staying simple to implement for legacy tool users. Mixed-signal design entry, design debug, simulation management, analysis, and reporting are all available in the Custom Compiler design environment. 
- Custom Compiler enhances efficiency with its visually-assisted automation flow and delivers quick and user-friendly polygon editing tools. Compiler detect physical and electrical faults during layout. Design rule checking, electromigration checking, and resistance and capacitance extraction are just a few examples. With support for templates and early parasitic simulation, the Custom Compiler design environment makes it simple to convey design intent and reach analogue design closure.
- Synopsys Primewave is a comprehensive and flexible environment for simulation setup and analysis of analog, RF, mixed-signal design, custom-digital and memory designs within the Synopsys Custom Design Platform. This tool helped in various types of simulations of the above designed circuit.
- Synopsys 28nm PDK is the Synopsys 28nm Process Design Kit(PDK) was used in creation and simulation of the above designed circuit.

##  CMOS INVERTER


<p align="Center">
  ![image](https://user-images.githubusercontent.com/71437573/155837779-458627a2-77d0-43c5-b375-1405e7c44b19.png)
<br />
  NOT GATE SCHEMATIC<br />
  
</p>


##  CMOS 2 Input AND Gate
##  CMOS 3 Input AND Gate
##  CMOS 3 Input OR Gate
##  CMOS XNOR Gate

