# Lab 3: Transistors as Switches

* Alexis Puckett 
* Hannah Markwell
  
January 25, 2024

# Project Summary:

The goal of this lab is to learn more about transistors and diodes. In this lab we analyzed a bipolar junction transistor, specifically, a TIP31C transistor. We built three different circuits consisting of a DC Power Supply, a breadboard, resistors, diodes, a switch, and the TIP31C transistor. The first circuit contained a 270 Ohm resistor with a LED and a switch. This circuit showed us the differences in voltage drop across and current through components when the switch was opened versus closed. We can see that an open switch causes an open circuit because the current through the components went to zero. The second circuit contained two resistors with an LED, transistor, and a switch. We measured the voltage drops and currents through the components in this circuit. We found that the current through the LED was the same in both the first and second circuits. We also found the voltage drop (Vce) across the transistor to be 0.015 V which is significantly smaller than the 1.2 V which occurs with saturation, so the transistor in this circuit was working in its active region and functioning as it should. Finally, the third circuit we constructed consisted of two resistors with an LED, transistor, and a potentiometer instead of the switch. We changed the resistance of the potentiometer to see how it affected the brightness of the LED and took measurements of the voltage drops and currents through the components at different levels of brightness to see how these values change with changing the resistance of the potentiometer... add results of this circuit

# Design/Methods:

For this lab we needed:
* Digital Multi-meter (DMM): Fluke 87
* DC Power Supply: Global Specialties 1403
* Resistors with resistances 2.2Ohms, 270Ohms, and 1kOhms
* An LED
* Sliding switch from the Sparkfun kit
* Electric motor from the Sparkfun kit
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

The first circuit consisted of a resistor (R1) in series with an LED in series with a switch on a breadboard. 

<p align="center">
  <img src="https://github.com/elibarrow/BAE305-SP24-Lab2/blob/main/Series%20Circuit%20Schematic.png">
</p>

Once we put all of the components together on the breadboard, we supplied 5V to the circuit using the DC Power Supply (DCPS). We then used the Digital Multi-Meter (DMM) to measure the voltage at each test site (T1, T2, T3, and T4) seen on the circuit drawing. We recorded the values and measured the voltage drop across each component in this circuit and the current through the LED using the DMM.

### Circuit Two:

The second circuit consisted of two resistors (R1 and R2), an LED, a TIP31C transistor, and a switch. Once built on the breadboard, we connected it to the DCPS to supply 5V to the circuit.

<p align="center">
  <img src="https://github.com/elibarrow/BAE305-SP24-Lab2/blob/main/Series%20Circuit%20Schematic.png">
</p>


We then measured the voltage at each test point (T1-T7) and the voltage drop across each component along with the current through the LED and R2. Finally, we adjusted the fine control on the DCPS to see what happens to the current through the transistor as the voltage changes.

### Circuit Three: 

The final circuit contained two resistors (R1 and R2), an LED, a TIP31C transistor, and a potentiometer on a breadboard. Once assembled we once again connected it to the 5VDC of the DCPS.

<p align="center">
  <img src="https://github.com/elibarrow/BAE305-SP24-Lab2/blob/main/Series%20Circuit%20Schematic.png">
</p>

We measured the voltages using the DMM at each point labeled in drawing (T1-T6). We then changed the resistance in the potentiometer until the LED was barely visible and took measurements. These are the Dim LED measurements. Then we changed the resistance in potentiometer until the LED reached full brightness and took measurements. These are the Bright LED measurements. Next, we found three levels of brightness with voltages between the Dim and Bright LED voltage measurements and took measurements at these three levels. 

We were unable to complete part two of the lab because we ran out of time and we could not get the motor to work. We then realized that the resistor we were using had too high of a resistance and was taking too much voltage. We used the 270 ohm resistor instead of the 2.2 ohm resistor.

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

Voltage drop (Vce) across the transistor (Q1) when the LED is on:
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
| R2      | 0.005 V  | 0.199 V | 0.032 V  | 0.05 V  | 0.024 V  |

Measured Current Through Components and Gain

| Component | Current (Dim LED) | Current (Bright LED) | Current (Midpoint 1) | Current (Midpoint 2) | Current (Midpoint 3) |
|:---:|---|---|---|---|---|
| LED 1 (Ic)   | 0.01 mA  | 10.66 mA |  3.02 mA  | 4.73 mA |  2.09 mA |
| R2 (Ib)      | 0.01 mA  | 0.27 mA  | 0.03 mA   | 0.04 mA | 0.01 mA  |
| Gain (Ic/Ib) | 1        | 29.4     |  151      |  118.25 |  209     |

Calculated Current Through Components

| Component | Current (Dim LED) | Current (Bright LED) | Current (Midpoint 1) | Current (Midpoint 2) | Current (Midpoint 3) |
|:---:|---|---|---|---|---|
| R1       | 0.355 mA   | 10.83 mA  |  2.95 mA   | 4.74 mA  |  2.08 mA |
| R2 (Ib)  | 0.0051 mA  | 0.201 mA  | 0.032 mA   | 0.051 mA | 0.024 mA |

# Discussion Questions:

## Discussion Question One:
How does the current through the LED compare between circuits 1 and 2?

The current through the LED in circuits 1 and 2 was exactly the same for each current. When the switch was closed the current was measured to be 10.89mA, and when the switch was open the current was 0.01mA. 

## Discussion Question Two:
The datasheet mentions a maximum voltage drop (VCE) of 1.2V at saturation. We would like a much smaller value, such as the fraction of a volt that you measured in the first circuit across the switch, S1, when it is on. How does your measured VCE compare to the one listed in the datasheet? Do you think we are operating this transistor in the saturation region?


# Conclusions:

In this lab we learned about diodes and transistors. Our learnings were discovered by constructing a series of circuits and placing differing transistors and diodes into the circuits. These circuits allowed us to see how diodes are semiconductors and stop current flow from one direction by using LED’s to see the current and voltage flow/drop. This also showed, by using a switch and potentiometer, how diodes and LED’s control current flow in one direction in circuit. In addition, in this lab we learned how transistors can be used as a switch in certain circuits, we saw this by using a series of differing transistors such as a TIP 31 C transistor, a 1kOhm trimmer potentiometer and a switch from the SparkFun kit. These allowed us to control the current that was going through the transistors. With these transistors, the lab also showed us how we can control the current and voltage going through each of the components. The current and voltage were measured and we also saw how the transistors take some of the current away from the rest of the components and limit how much is going through. 
