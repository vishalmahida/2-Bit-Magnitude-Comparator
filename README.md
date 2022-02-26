# 2-Bit-Magnitude-Comparator

The design of a 2-bit magnitude comparator utilizing Synopsys Custom Compiler on 28nm CMOS technology is shown in this repository.

##  Table of Content
   * [Abstract](#Abstract)
   * [Introduction](#Introduction)
   * [Detailed Explanation](#Detailed-Explanation)
   * [Tools Used](#Tools-Used)
   * [CMOS INVERTER](#CMOS-INVERTER)
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

