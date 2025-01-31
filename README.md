# Bandoja---Portfolio
Completion requirement for course COSC 111B - CS ELECTIVE 3 (Internet of Things)

LabActivity 1 - objective is to create a running light from right to left using digitalWrite().
- using pins 8 to 12 for LED
- turn LED ON starting from pin 12 to 8
- after all LED is on, then turn LED OFF starting from pins 12 to 8

LabActivity 2 - objective is to add brightness control to the output of LabActivity1.
- using the output of LabActivity1
- use analogWrite() to create a fade effect.
- using while loop to repeatedly put increment to analogWrite() to slowly increase or decrease the brightness of each LED when turning ON or OFF.

LabActivity 3- objective is to imitate a fire detector using photoresistor and thermistor, however, since tinkercad doesn't have thermistor, a temperature sensor was substituted.
- Temperature sensor is at pin A0
- Photoresistor is at pin A2
- LED is at pin 12
- using map() function to transform the analog reading values to digital values
- using analogRead() to photoresistor and temperature sensor to get input from sensors.
- when a certain threshold set in photoresistor and temperature sensor is met then an LED will blink ON and OFF.


LabActivity 4 - objective is to use photoresistor that will sense light and when a certain threshold is met, then an LED will blink ON and OFF, and when typed "stop" in serial monitor, regardless of casing then it will stop functioning.
- 
