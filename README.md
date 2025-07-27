COMPANY:CODTECH IT SOLUTIONS 
NAME:MARILAKSHMI S 
INTERN ID:CT04DH848
DOMAIN:EMBEDDED SYSTEMS 
DURATION:4 WEEKS
# Task-1-Temperature-Monitor-using-LCD
This project reads ambient temperature using the TMP36 analog temperature sensor and displays the temperature on a 16x2 character LCD (no I2C). The LCD shows real-time temperature in Celsius with two decimal precision.

 Components Used
- Arduino UNO
- TMP36 temperature sensor
- 16x2 LCD display (non-I2C)
- Potentiometer (10kΩ) – for LCD contrast
- Breadboard and jumper wires

Circuit Connections

TMP36:
- VCC → 5V  
- GND → GND  
- OUT → A0  

LCD to Arduino (4-bit mode):

LCD Pin | Function | Arduino Pin 
 1 (VSS) | GND | GND 
 2 (VDD) | +5V | 5V 
 3 (VO) | Contrast | Pot middle
 4 (RS) | Register Select | D12 
 5 (RW) | Read/Write | GND 
 6 (E) | Enable | D11 
 11 (D4) | Data | D5 
 12 (D5) | Data | D4 
 13 (D6) | Data | D3 
 14 (D7) | Data | D2 
 15 (A) | Backlight + 5V 
 16 (K)  Backlight –  GND 

The system operates by converting ambient temperature into an analog voltage using the TMP36 temperature sensor. This analog voltage is read by the Arduino’s analog pin (A0) and then converted into a temperature value using a mathematical formula. The calculated temperature is then displayed on a 16x2 LCD screen using 4-bit data communication.
