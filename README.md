#GRBL 28byj-48

This is a modified fork from ruizivo/GRBL-28byj-48-Servo.  This modification implements all 3-axises XYZ to a 28BYJ-48 stepper motor.

The motors (28byj-48) are connected to a controller card (Arduino UNO or Nano) that uses the chip ULN2003. This board is connected to pins.

| Axis       | Arduino      |ULN2003|ULN2003|28BYJ-48|
|:----------:|:------------:|:-----:|:-----:|:------:|
| X-Axis     |      D5      |IN1    |OUT1   |BLUE    |
|            |      D4      |IN2    |OUT2   |PINK    |
|            |      D2      |IN3    |OUT3   |YELLOW  |
|            |      D2      |IN4    |OUT4   |ORANGE  |
| Y-Axis     |      A0      |IN1    |OUT1   |BLUE    |
|            |      A1      |IN2    |OUT2   |PINK    |
|            |      A2      |IN3    |OUT3   |YELLOW  |
|            |      A3      |IN4    |OUT4   |ORANGE  |
| Z-Axis     |      D13     |IN1    |OUT1   |BLUE    |
|            |      D12     |IN2    |OUT2   |PINK    |
|            |      D9      |IN3    |OUT3   |YELLOW  |
|            |      D8      |IN4    |OUT4   |ORANGE  |
|            |              |       |+5V    |RED     |


This work was derived from:
See https://github.com/ruizivo/GRBL-28byj-48-Servo

#GRBL 28byj-48 + Servo Motor

This GRBL uses an ugly hack to control two motors unipolar steps as 28byj-48 and also supports a servo motor on pin 11

The motors (28byj-48) are connected to a controller card that uses the chip ULN2003. This board is connected to pins A0, A1, A2, A3 for the Y axis and 2,3,4,5 digital pins to the axis X. The servomotor connected to pin 11 h.

Credits to robottini who did support the servo motor ... link to git https://github.com/robottini/grbl-servo

I tested the code very well with 328p (Arduino Uno, Duemilanove etv), not with 2560 (Arduino Mega) because I did not do the alterations in the file cpu_map_atmega2560.h



