# make_thime

# Objectives
This make project displays the time or the temperature & humidity, packed in a LEGO ® case.
(LEGO is a trademark of the LEGO Group)

![thime-case](https://user-images.githubusercontent.com/47274144/52938631-725cb280-3362-11e9-8f9e-697b81218b34.png)

## Solution
### Display
* the time hours & minutes in HH:mm 24h format.
* the temperature (Deg C) and Humidity (%RH).
* uses 4-Digits in red.
### Infrared Remote Control to set Mode
* [Button n] = [Mode]
* Button 1 = Display Time.
* Button 2 = Display Temperature + Humidity. No digits.
* Button 3 = Display Temperature with 2 digits.
* Button 4 = Display Humidity with 2 digits.
* Button 5 = Set Hours.
* Button 6 = Set Minutes.
* Button 7 = Set Brightness.
* Button 8 = Turn display on / off.
* Button 9 = N/A.
* Button - = Decrease Hours, Minutes, Brightness depending mode.
* Button + = Increase Hours, Minutes, Brightness depending mode.
_Notes_
* When powering on, the default time is 19:58. Set the time by pressing button 5 for hours and button 6 for minutes.
* Ensure to press button 1 after completing settings via buttons 5 - 9 and -/+.

### Creation Rules
* Use as microcontroller an Arduino UNO or compatible.
* Use standard LEGO bricks.
* Minimize LEGO brick modifications.
* LEGO Case with modular components.
* Build code with B4R.

## Hardware Parts (approx cost EUR)
* 1x Arduino UNO (8 EUR)
* 1x 4-Bit LED Digital Tube Model (2 EUR)
* 1x DHT22 temperature & humidity sensor (8 EUR)
* 1x IR Receiver with Remote Control (4 EUR)
* In addition for the prototype: Breadboard (2 EUR)
* LEGO bricks (10 EUR)

## Software
* Arduino IDE 1.8.0 or higher
* B4R 1.8.0 or higher

## Wiring
![thime_bb](https://user-images.githubusercontent.com/47274144/52938630-71c41c00-3362-11e9-93e2-abe14f3ce144.png)

```
LED Display = Arduino
CLK = Digital 8 (yellow)
DIO = Digital 7 (green)
VCC = 3.3v (red)
GND = GND (black)
DHT22 = Arduino
VCC = 5v (red)
DATA = Digital 4 (yellow)
GND = GND (black)
IR Receiver = Arduino
DATA = Digital 11 (purple)
VCC = 5v (red)
GND = GND (black)
(WireColors)
```

## Soure Code
The [B4R](https://www.b4x.com/b4r.html) source code and required libraries can be found in archive __thime.zip__. The code is well documented.
