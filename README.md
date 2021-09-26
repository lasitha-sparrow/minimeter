# Arduino based multi-meter

Welcome to the minimeter wiki!🥇

The whole project based on (https://www.instructables.com/member/VolosR/) little Nano based “semi” multi-meter solution on Instructables.com. and [stephans nanOmeter project](https://www.protowrxs.com/index.php/2020/01/01/nanometer-2020/)(Stephan/ProtoWrxs )

![](https://raw.githubusercontent.com/lasitha-sparrow/minimeter/main/WhatsApp%20Image%202020-12-06%20at%2009.54.26.jpeg)

## At this point the little box can:

* Measure DC voltage (with reverse voltage diode protection)
* Read an analog input and show the value, as well as the min, max and average values
* Measure the resistance of a resistor
* Measure the voltage drop of a diode or LED (and test the LED there too)
* Act as a beeping / LED continuity tester
* Generate a PWM output
* Test a servo
* Test a ping / SR04 sensor
* Drive a stepper motor driver\
* Monitor the external battery supply voltage on the Vin pin
* Allow adjustments to the data dump timer (more later)
* Do an I2C bus scan and show attached device addresses.
## Current pin uses are:

(P) = PWM Pin

* 0 – Rx – On header pin lower right – Used to receive commands from serial console, etc
* 1 – Tx – On header pin lower right – Dumps CSV data to here
* 2 – Left Button
* 3(P)- Middle Button (on interrupt)
* 4 – Right Button
* 5(P)- Software Servo Pin
* 6(P)- PWM output on three pin header
* 7 – Ping Trigger
* 8 – Ping Echo
* 9(P)- Stepper IN1
* 10(P)- Stepper IN3
* 11(P)- Stepper IN2
* 12 – Stepper IN4
* 13 – Used for speaker output and LED display
* A0 – Main Analog Input
* A1 – Voltage Meter input – on 100k/10k divider
* A2 – Input for Diode and Resistor testing
* A3 – SPARE
* A4 – I2C bus
* A5 – I2C bus
* A6 – SPARE
* A7 – spare

I used original servo library since stephans Adafruit’s SoftServo library as the normal servo library kills some PWM pins and I wasn’t sure if they would be needed.The AdaFruit OLED library is used for the SSD1306 device which is the 128 x 32 pixel version. VolsR’s updated version uses the larger 128×64 version but personally I would love the minimalistic compact look for this project. Aslo to avoid measurement reading error from the touch ,i applied thick layer of hot-glue to the back of the circuit board.

To add the images I “temporarily borrowed” some icon art from online (I’ll give them back when I’m done) and converted them to the HEX format needed using the handy image2cpp online at at https://diyusthad.com/image2cpp. Works great and good enough results for me.

