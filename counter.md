
**3-bit LED Binary Counter**

```.C
//Code for checking if the circuit is set up properly

//creating variables for each LED
int pin2 = 2;
int pin3 = 3;
int pin4 = 4;
int pin5 = 5;

void setup()
{
pinMode(pin2, OUTPUT);
pinMode(pin3, OUTPUT);
pinMode(pin4, OUTPUT);
pinMode(pin5, OUTPUT);
}

void loop()
{
//Turning all the LED lights on
digitalWrite(pin2, HIGH);
digitalWrite(pin3, HIGH);
digitalWrite(pin4, HIGH);
digitalWrite(pin5, HIGH);
}
