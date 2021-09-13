# uPython-ESP32-HWTest
Simple generic platform to preform hardware test with ESP32 running uPython build. Input is the HW and output is .csv (columns: testId, testName, testType, testOutput, testComment(can be Json string to accomodate multiple values like min/max, reff, etc..)) in webserver (client mode, the test result Ip is printed into USB serial)

# Examples
## DS Apollo One (3)
Examples/DS_Apollo1_3
16LED RGBW fixture, 100W nominal, DS Voyager Power (20V, DoDC, Underwater compatible)
* 1xRGBW output
* LM75 temp sensor
* uSD card reader / 8GB Card
* 2x Buttons (one to wake from deep sleep)
* Fan Output (and PWM read)
* IMU

## DS Spot (02)
Examples/DS_Spot_02
[Schematic](url)
1LED RGBW 10W Nominal ultra narrow spotlight, USBC (USB2, 5V 2A max)
* 1xRGBW {r:33,g:25,b:26,w:,27}
* Ressistor temp sensor {32}
* uSD card reader / 8GB Card {sck:14/18,mosi:15/23,miso:12/19,cs:13/5} [slot2/slot3](https://docs.micropython.org/en/latest/library/machine.SDCard.html)
* 2x Buttons (one to wake from deep sleep) {power:34,program:35}
