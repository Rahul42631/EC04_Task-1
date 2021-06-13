# Roll OVA
## Troubleshooting
We can break the code into smaller parts in order to avoid last minute error which would lead us to go through whole code and circuit testing.
TESTING INDIVIDUAL ELEMENTS
1. Getting input from rotary encoder via arduino and displayion on Serial Monitor.
2. Measuring distance from distance sensor and printing it on LCD display.

### 1. Testing Roatry encoder

![Rotary-Encoder-Pinout](https://user-images.githubusercontent.com/82231782/121569977-032d8f80-ca3f-11eb-8840-8a98afeabba4.jpg)
In this the value of count decreases if the rotatry encoder is rotated counter clockwise and increases if rotated clockwise.We can find the angle covered per increase in value of count hence we can find the distance covered by the roller.

Connections
OUTPUT A - Pin 4
OUTPUT B - Pin 5
 Code:-
```
int counter=0,New,Prev;

void setup()
{
pinMode(4,INPUT);
pinMode(5,INPUT);
Serial.print(9600);
}
void loop()
{
New=digitalRead(4);
if(New!=Prev)
{
if(digitalRead(5)!=New)
count--;        
else
count++;
}
Serial.print(count);
Prev=New;
}
```
### 2. Testing LCD display

CIRCUIT

![Untitled](https://user-images.githubusercontent.com/82231782/121810666-5db52e80-cc7f-11eb-945a-d1f5ab60286e.png)

Using LCD without resistor might burn the LCD display.

Connect the pins as per given in the diagram.

Code:-

```
#include<LiquidCrystal.h>
LiquidCrystal r(7,8,9,10,11,12);
int trigger=4,echo=3,Time;
void setup() {
  pinMode(trigger,OUTPUT);
   pinMode(echo,INPUT);
  r.begin(16,2);
  Serial.begin(9600);
}

void loop() {
 digitalWrite(trigger,HIGH);
 delayMicroseconds(10);
   digitalWrite(trigger,LOW);
   delayMicroseconds(10);
   digitalWrite(trigger,HIGH);
 delayMicroseconds(10);
   digitalWrite(trigger,LOW);
   
   Time=0.007*pulseIn(echo,HIGH);
   delay(25);
   Serial.println(Time);
  
r.setCursor(0,0);
r.print(Time);
 
}
```

