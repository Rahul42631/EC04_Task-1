# 15 Project 
## 1. Roll OVA (compact digital rolling ruler)
Aim is to build a distance measuring device using rotary encoder and display the measured distance on LCD display using an Arduino.
### Working:-
Here the mechanical rotational motion is turned into digital signals from which we can get the information like angular velocity ,direction of rotation , angular displacement.These signals are sent to arduino which calulate and display the length covered on LCD display.
![download](https://user-images.githubusercontent.com/82231782/121404658-c51a6800-c979-11eb-8580-8326c803431c.jpg)
### Use:-
Compact and easy to carry.

Can measure the length of curved path also.

![5cow8e](https://user-images.githubusercontent.com/82231782/121411890-b932a400-c981-11eb-968d-1dfc2d8c2501.gif)

## 2. 8x8x8 LED cube
Building 8x8x8 LED cube which forms 3D pattern and visual effects using Arduino.
### Working:-
Consider a 8x8 LED here we can't operate all the LED's at the same time using 16 pins only hence leds are glown line by line at a very fast which looks like a 2D pattern due to persistance of vision. Similar concept is applied in 8x8x8 LED cube where 8x8 led planes are grown at a very fast rate formimg a 3D pattern.

![images](https://user-images.githubusercontent.com/82231782/121416881-f0578400-c986-11eb-81b6-dc1107211b6e.jpg)
### Use:-
Can be used to plot 3D graph.

Can be used for creating 3D visual effects for decoration.

![5cmep5](https://user-images.githubusercontent.com/82231782/121416521-85a64880-c986-11eb-8b67-8c98deb9f842.gif)

## 3. ImagiCharm
Create an 8x8 RGB LED grid forming patterns which are customizable using Mobile App cia USB
### Working:-
Since we can't operate all the LED's at the same time using 16 pins only hence leds are glown line by line at a very fast which looks like a 2D pattern due to persistance of vision.

![images](https://user-images.githubusercontent.com/82231782/121417696-cf436300-c987-11eb-9fdd-e11619048a99.jpg)


### Use:-
Costomizable fashion accessories that looks very atrective.

Easy to carry and can play simple games on it like snake.

![images](https://user-images.githubusercontent.com/82231782/121418100-3cef8f00-c988-11eb-96b7-17671c9b5c61.jpg)

## 4. Gas Leakage Detector
Aim is to create a device which can sence the increase in concentration of gas and alarm everyone using a buzzer via Arduino.

### Working:-
The ability to detect gas and the type of gas depends upon chemiresistor (substance that changes its resistance due to change in chemistry of environment). Most commonly used chemiresistor is SnO2 which is an n-type semiconductor that has free electrons which are attracted to the surface by o2 present in air which lead to decrease in conductivity of the material when the concentratio of another gas increases the concentration of O2 in air decreases hence the electrons start taking part in conduction .A pre configured comparator reacts to the voltage change which is interpreted by Arduino which operates the buzzer accordingly. 

![Gas-Sensor-Working-Principle](https://user-images.githubusercontent.com/82231782/121419885-17fc1b80-c98a-11eb-8dd7-7d8a2e60acff.gif)       ![download](https://user-images.githubusercontent.com/82231782/121419897-1af70c00-c98a-11eb-84a4-d555e14dbb9c.jpg)
### Use:-
Can avoid fatal accidents due to gas leakage.

Can be used to get information of concentration of pollutent in air of a specific area.

## 5. Smart Door
Aim is to start recording video using Raspberry pi when ever the PIR sensor detects any motion near it.
### Working:-
PIR Sensor consist of Pyroelectric sensor which generates energy when eposed to heat which means IR rays emitted by human or animal body gets detected by PIR sensor whenever PIR Sensor detects any motion it supples 3V Voltage at the output pin else it stays at zero voltage.Raspberry pi keeps the record of this voltage change and starts recording video via camera whenever PIR sensor detects any motion. 

![download](https://user-images.githubusercontent.com/82231782/121521045-3a854780-ca11-11eb-8efd-ee3c9a2e20b5.png)
### Use:-
Security.

This system can also be used by photographers.

## 6. Hand gesture controlled car
Building a RC car that can be controlled by hand gestures using Esp32 (Inbuild gyroscope sensor).

![5cmyv9](https://user-images.githubusercontent.com/82231782/121522066-5ccb9500-ca12-11eb-8bc6-7af04ea31852.gif)
### Use:-
Similar concept could be appiled to build automatic wheel chairs.

## 7. IOT driven water tank system
Making an IOT driven Water tank system which can open and close water supply valves, detects the level of waer filled and communicate all this data through smart phone using TOF10120 distance sensor and esp32.

![download](https://user-images.githubusercontent.com/82231782/121524601-16c40080-ca15-11eb-8ae0-2cc5ccb5a06d.jpg)
### Use:-
Close the value when water reaches configured level and prevent overflowing. 

## 8. Voice controlled lights and fans
Automating hoome appliances starting with fans and led lights.IOT allows us to communicate the data from anywhere using smartphones and microcontrollers control the electric appliances.

![download](https://user-images.githubusercontent.com/82231782/121527204-ca2df480-ca17-11eb-9bc7-e38fe81aa20f.jpg)
### Use:-
Allow us to keep the data of electrical appliances under operation and sometimes can avoid accidents.

## 9.Real time virtual piano using hand gestures
Playing piano by keeping the track of fingers movement using microcontrolles and speaker connected via bluetooth.

![images](https://user-images.githubusercontent.com/82231782/121527394-fc3f5680-ca17-11eb-8dbc-2dd6e9c43568.jpg)
## Use:-
Easy to carry and compact.

