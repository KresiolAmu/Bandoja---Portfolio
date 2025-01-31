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
- - using analogRead() to photoresistor and temperature sensor to get input from sensors.
- using map() function to transform the analog reading from sensors to digital values
- when a certain threshold set in photoresistor and temperature sensor is met then the LED will blink ON and OFF.


LabActivity 4 - objective is to use photoresistor that will sense light and when a certain threshold is met, then an LED will blink ON and OFF, and when typed "stop" in serial monitor, regardless of casing then it will stop functioning.
- Photoresistor is at pin A2
- LED is at pin 13
- using map() function to transform the analog reading from photoresistor to digital values.
- when a certain threshold is met, then the LED will blink
- using Serial.available() function to read inputs from serial monitor
- when typed "stop", regardless of casing, the code will halt functioning.

LabActivity 5 - objective is to create a circuit that will provide a connection through fastapi, and those who will connect can control the LED of the circuit to turn ON and OFF.
- The **arduino code** functions that when it receive an input value of '1' then the LED will turn ON. When input received is '0' then LED will turn OFF.
- The **python code** enables controlling of the arduino and establishing connection using fastapi.
- In startup event, it attempts to connect to the arduino with time.sleep(2) to ensure that the connection is fully opened up.
- In shutdown event, it simply closes the connection to the arduino
- In POST LED ON, when the fastapi receives a request to turn ON, then it will pass a byte string '1' to the arduino which will trigger the LED to turn on.
- In POST LED OFF, when the fastapi receives a request to turn OFF, then it will pass a byte string '0' to the arduino which will trigger the LED to turn off.

LabActivity 6 - 
