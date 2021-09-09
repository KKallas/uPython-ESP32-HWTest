# uPython-ESP32-HWTest
Simple generic platform to preform hardware test with ESP32 running uPython build. Input is the HW and output is .csv (columns: testId, testName, testType, testOutput, testComment(can be Json string to accomodate multiple values like min/max, reff, etc..)) in webserver (client mode, the test result Ip is printed into USB serial)

# Examples
## DS Apollo One (3)
Examples/DSApollo1_3
16LED RGBW fixture, 100W nominal, DS Voyager Power (20V, DoDC, Underwater compatible)
* 1xRGBW output
* LM75 temp sensor
* uSD card reader / 8GB Card
* 2x Buttons (one to wake from deep sleep)
* Fan Output (and PWM read)
* IMU

## DS Spot (2)
Examples/DSSpot_2
1LED RGBW 10W Nominal ultra narrow spotlight, USBC (USB2, 5V 2A max)
* 1xRGBW temp sensor
* Ressistor temp sensor
* uSD card reader / 8GB Card
* 2x Buttons (one to wake from deep sleep)
