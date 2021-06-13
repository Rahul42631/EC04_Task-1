# Gas Leakage Detection
## Problem Statement
Aim is to create a device which can sense the increase in concentration of gas and print it on a LCD display if the consentration gets higher then safty level it will alarm everyone using a buzzer via Arduino.

## Ideation and Planning
COMPONENTS USED IN PROJECT
Gas Sensor --> Microcontroller --> Buzzer

1. Gas sensor 
The MQ-2 smoke sensor is sensitive to smoke and to the following flammable gases:

-LPG

-Butane

-Propane

-Methane

-Alcohol

-Hydrogen

Working:-The ability to detect gas and the type of gas depends upon chemiresistor (substance that changes its resistance due to change in chemistry of environment). Most commonly used chemiresistor is SnO2 which is an n-type semiconductor that has free electrons which are attracted to the surface by o2 present in air which lead to decrease in conductivity of the material when the concentratio of another gas increases the concentration of O2 in air decreases hence the electrons start taking part in conduction .A pre configured comparator reacts to the voltage change which is interpreted by Arduino which operates the buzzer accordingly.

(MQ-2![MQ2-Gas-Sensor-Output](https://user-images.githubusercontent.com/82231782/121813425-9d811380-cc89-11eb-8592-a174c3878e72.gif)
)

2. Arduino nano Microcontroller
Since Arduino serves many more functionalities using it will increase the net cost of the project andding to that it will be bulky.
3. Pizo Buzzer
5. LCD display

Gas Sensor --> Microcontroller --> Buzzer + LCD DISPLAY

For different concentration of Gas the gas sensor will give differnt output values (0-5 voltage is mapped in 0-1023) which is read by arduino and displayed on LCD display and when the concentration gets above safety level the buzzer will start beaping.

APPROACH:-

After investigating through all the electrical componets ,circuits and PCB designes we can use fusion 360 ,Eagle,KiCad for designing mechanical structure and PCBs respectively. After coming up with efficient and compact designe it's time for prototyping phase.

## Prototyping
Keeping the over all cost of project in mind its time to implement the ideas by breaking project in smaller parts, if we find any undesired outcome we can go back to ideation stage and work recursively on the problem.




