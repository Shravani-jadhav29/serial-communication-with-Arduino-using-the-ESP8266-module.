# serial-communication-with-Arduino-using-the-ESP8266-module.

# Serial Communication with Arduino and ESP8266

This project demonstrates how to establish serial communication between an Arduino board and the ESP8266 Wi-Fi module for sending and receiving data.

## 🛠 Requirements

- Arduino Uno/Nano/etc.
- ESP8266 Wi-Fi module (e.g., ESP-01)
- Level shifter (or voltage divider) for TX pin (ESP8266 operates at 3.3V)
- USB to Serial adapter (if flashing ESP8266 separately)
- Arduino IDE


> ⚠️ **Note:** Connect ESP8266 RX through a voltage divider to avoid overvoltage (Arduino TX is 5V, ESP RX expects 3.3V).

## 🧠 Basic ESP8266 code Sketch

```cpp
void setup() {
 Serial.begin(9600);
 delay(1000);
Serial.print("serial communication text start");

}

void loop() {
  
Serial.println("Hello");
delay(1000);

}
