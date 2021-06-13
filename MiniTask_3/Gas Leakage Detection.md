# Gas Leakage Detection

TESTING THE CODE FOR EACH COMPONENTS INDIVIDUALLY TO VERIFY THE PROPER WORKING OF CODE AND COMPONENTS
1.Testing the working of Gas sensor and buzzer.
2. Testing the proper working of LCD by measuring distance from distance sensor and printing it on LCD display.

## 1.Testing the working of Gas sensor and buzzer

![Untitled3](https://user-images.githubusercontent.com/82231782/121816003-c9ef5c80-cc96-11eb-94c0-071b0e31f1e6.png)

Code for corrosponding circuit
```
void setup()
{ 
  pinMode(13, OUTPUT);
  pinMode(A0,INPUT);
  Serial.begin(9600);
}

void loop()
{
  Serial.println(analogRead(A0));
 
 
 if(analogRead(A0)>700)
 {
  
   digitalWrite(13,HIGH);
 }
 else
 { digitalWrite(13,LOW);
   
 }
 
}

```

## 2. Testing LCD display

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
The final designe we want to achieve(Follow the circuit of given code)

![Untitled2](https://user-images.githubusercontent.com/82231782/121815896-40d82580-cc96-11eb-913d-08a5d9f662ec.png)

```
#include<LiquidCrystal.h>
LiquidCrystal r(7,8,9,10,11,12);

void setup()
{ r.begin(16,2);
  pinMode(13, OUTPUT);
  pinMode(A0,INPUT);
  Serial.begin(9600);
}

void loop()
{r.setCursor(0,0);
  Serial.println(analogRead(A0));
 
 
 if(analogRead(A0)>700)
 {
   r.print(analogRead(A0));
   r.setCursor(0,1);
   r.print("DANGER");
   digitalWrite(13,HIGH);
 }
 else
 { digitalWrite(13,LOW);
   r.print(analogRead(A0));
 }
 delay(500);
 r.clear();
}
```



