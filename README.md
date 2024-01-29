# Lab 3: Transistors as Switches

* Alexis Puckett 
* Hannah Markwell
  
January 25, 2024

# Project Summary:


# Design/Methods:

For this lab we needed:
* Digital Multimeter (DMM)
* DC Power Supply
* Resistors with resistances 2.2Ohms, 270Ohms, and 1kOhms
* An LED
* Sliding switch
* Electric motor
* NTE 125 diode
* 1kOhm trimmer potentiometer
* A TIP31C transistor

First, measure resistor values using Fluke DMM to compare to labeled resistance and to use in calculations.

| Resistor| Nominal Value| Actual Value |
|:---:|---|---|
|  R1    | 270 &Omega;  |  267.7 &Omega; |
| R2     | 1 k&Omega;   | 988 &Omega;    |
| R3     | 2.2 &Omega;  |  2.3 &Omega;   |


### Circuit One:
resistor in series with an LED in series with a switch on a breadboard




# Results:

### Circuit One Results:

Measured Voltage at Each Test Point

| Test Point | Voltage (Switch On) | Voltage (Switch Off) |
|:---:|---|---|
|   T1   | 4.999 V  | 4.991 V |
| T2     | 2.067 V  | 4.99 V  |
| T3     | 0.002 V  |  3.49 V |
| T4     | 0.007 V  | 0.002 V |

Measured Voltage Across Components

| Component | Voltage (Switch On) | Voltage (Switch Off) |
|:---:|---|---|
|   R1   | 2.94 V   | 0 V      |
| LED 1  | 2.047 V  | 0.147 V  |
| S1     | 0.001 V  |  0.001 V |

Current Through Components (Measured and Calculated)

| Component | Current (Switch On) | Current (Switch Off) |
|:---:|---|---|
|   R1 (calculated) | 10.98 mA  | 0 mA    |
| LED 1 (measured)  | 10.89 mA  | 0.01 mA |

### Circuit Two Results:

Measured Voltage at Each Test Point

| Test Point | Voltage (Switch On) | Voltage (Switch Off) |
|:---:|---|---|
|   T1     | 4.92 V   | 4.99 V  |
| T2       | 2.061 V  | 4.99 V  |
| T3 (Vce) | 0.015 V  |  3.47 V |
| T4       | 0 V      |     0 V |
| T5 (Vbe) | 0.696 V  | 0.009 V |
| T6       | 4.97 V   | 0.007 V |
| T7       | 4.99 V   |  4.99 V |

Measured Voltage Across Components

| Component | Voltage (Switch On) | Voltage (Switch Off) |
|:---:|---|---|
|   R1   | 2.92 V   | 0 V      |
| LED 1  | 2.047 V  | 0.005 V  |
| R2     | 4.27 V   |  0 V     |
| S1     | 0.001 V  |  0 V     |

Current Through Components (Measured and Calculated)

| Component | Current (Switch On) | Current (Switch Off) |
|:---:|---|---|
|   R1 (calculated)    | 10.98 mA  | 0 mA    |
| LED 1 (measured)(Ic) | 10.89 mA  | 0.01 mA |
| R2 (measured)(Ib)    | 4.36 mA   | 0.01 mA |
| R2 (calculated)      | 4.32 mA   | 0 mA    |

What is the voltage drop (Vce) across the transistor (Q1) when the LED is on?
Vce = 0.015 V

What should you see happen to Ic as you change the voltage?

* At V= 5.5V, Ic = 12.63 mA
* At V= 5.4V, Ic = 12.23mA
* At V= 5.3V, Ic = 11.9mA
As we increase voltage, the Ic increases.

### Circuit Three Results:

Measured Voltage at Each Test Point

| Test Point | Voltage (Dim LED) | Voltage (Bright LED) | Voltage (Midpoint 1) | Voltage (Midpoint 2) | Voltage (Midpoint 3) |
|:---:|---|---|---|---|---|
|   T1     | 4.97 V  | 4.99 V  |        |         |        |
| T2       | 4.89 V  | 2.05 V  | 4.37 V | 3.67 V  | 4.49 V |
| T3 (Vce) | 3.09 V  | 0.001 V | 2.47 V | 1.74 V  | 2.54 V |
| T4       | 0 V     |     0 V |        |         |        |
| T5 (Vbe) | 0.54 V  | 0.669 V | 0.58 V | 0.605 V | 0.583 V|
| T6       | 0.54 V  | 2.65 V  | 0.613 V| 0.655 V | 0.605 V|

Measured Voltage Across Components

| Component | Voltage (Dim LED) | Voltage (Bright LED) | Voltage (Midpoint 1) | Voltage (Midpoint 2) | Voltage (Midpoint 3) |
|:---:|---|---|---|---|---|
|   R1    | 0.095 V  | 2.9 V   |  0.79 V  |  1.27 V |  0.557 V |
| LED 1   | 1.78 V   | 2.04 V  | 1.901 V  | 1.95 V  | 1.88 V   |
| R2      | 0.005 V  | 1.99 V  | 0.032 V  | 0.05 V  | 0.024 V  |

Measured Current Through Components and Gain

| Component | Current (Dim LED) | Current (Bright LED) | Current (Midpoint 1) | Current (Midpoint 2) | Current (Midpoint 3) |
|:---:|---|---|---|---|---|
| LED 1 (Ic)   | 0.01 mA  | 10.66 mA |  3.02 mA  | 4.73 mA |  2.09 mA |
| R2 (Ib)      | 0.01 mA  | 0.27 mA  | 0.03 mA   | 0.04 mA | 0.01 mA  |
| Gain (Ic/Ib) | 1        | 29.4     |  151      |  118.25 |  209     |

Calculated Current Through Components

| Component | Current (Dim LED) | Current (Bright LED) | Current (Midpoint 1) | Current (Midpoint 2) | Current (Midpoint 3) |
|:---:|---|---|---|---|---|
| R1       | 0.01 mA  | 10.66 mA |  3.02 mA  | 4.73 mA |  2.09 mA |
| R2 (Ib)  | 0.01 mA  | 0.27 mA  | 0.03 mA   | 0.04 mA | 0.01 mA  |





# Discussion Questions:

## Discussion Question One:
How does the current through the LED compare between circuits 1 and 2?

## Discussion Question Two:
The datasheet mentions a maximum voltage drop (VCE) of 1.2V at saturation. We would like a much smaller value, such as the fraction of a volt that you measured in the first circuit across the switch, S1, when it is on. How does your measured VCE compare to the one listed in the datasheet? Do you think we are operating this transistor in the saturation region?


# Conclusions:
