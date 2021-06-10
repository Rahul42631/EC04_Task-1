# Roll OVA
## Troubleshooting
Trouble shooting can be categorized under 2 sub parts
1. Getting input from rotary encoder via arduino and displayion on Serial Monitor.
2. Displaying Input from serial monitor on LED display.

### 1. Testing Roatry encoder

![Rotary-Encoder-Pinout](https://user-images.githubusercontent.com/82231782/121569977-032d8f80-ca3f-11eb-8840-8a98afeabba4.jpg)
```
int counter=0,New,Prev;

void setup()
{
pinMode(4,INPUT);
pinMode(5,INPUT);
Serial.print(9600);
}
```
