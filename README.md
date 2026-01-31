# Buck-Converter-using-OpAmp-and-SR-Latch
#Project Overview
In this project , we have implemented a DC-DC Buck Converter using Nmos as switching device,Comparator based PWM generator,and SR latch control. The system output is regulated ( has little noise) by giving feedback to comparator and checks for deviation and more the deviation, width of PWM generator is more which is fed to SR latch which helps in switching ON and OFF the transistor and the design is build in Ltspice

#Objective 
1.Building Buck converter system using Diode,Inductor,capacitor and resistors
2.Generating PWM using comparator
3.Implement closed loop voltage regulation.
4.Analyzing Transient and Steady State behaviour.

#System Block-wise Description
-Input supply (20V0
-NMOS as power switching device 
-Freewheeling diode (D1) for ensuring inductor current continuity after switched OFF 
-LC Filter to smooth out output voltage
-Resistors for load conditions.

#Output sensing and FeedBack Network
Shunt resistor(R9= 0.1 ohms) for current sensing
Output voltage divider(R6 and R7) for output scaling

#Error Amplification 
operational amplifier as error amplifier
RC Compensation network (R8 and C2)

#PWM generation
Comparator (LT1011)
Carrier signal: used both sine and pulse.

#SR Latch configurations
Set input: PWM comparator output
Reset input: Clock pulse

#Working Principle (Step-by-Step)
1.The input DC voltage is applied to the buck converter.
2.The comparator generates a PWM signal based on feedback error.
3.The SR latch processes PWM pulses, removing glitches.
4.The NMOS switches ON/OFF according to the latch output.
5.The inductor stores and releases energy, smoothing current flow.
6.The LC filter converts the switching waveform into DC output.
7.The feedback loop continuously adjusts duty cycle to regulate output voltage. 

#Applications
DC–DC voltage regulators
Power management systems
Embedded and industrial power supplies
Educational demonstration of analog control loops
