---
title: Grove - Rotary Angle Sensor
category: Sensor
bzurl: https://seeedstudio.com/Grove-Rotary-Angle-Sensor-p-770.html
oldwikiname: Grove_-_Rotary_Angle_Sensor
prodimagename: Grove-Rotary_Angle_Sensor.jpg
bzprodimageurl: http://statics3.seeedstudio.com/images/101020017 1.jpg
surveyurl: https://www.research.net/r/Grove-Rotary_Angle_Sensor
sku: 101020017
tags: grove_analog, io_3v3, io_5v, plat_duino, plat_linkit, plat_bbg, plat_wio, plat_pi
---

![](https://github.com/SeeedDocument/Grove-Rotary_Angle_Sensor/raw/master/img/rotary.jpg)

The rotary angle sensor produces analog output between 0 and Vcc (5V DC with Seeeduino) on its D1 connector. The D2 connector is not used. The angular range is 300 degrees with a linear change in value. The resistance value is 10k ohms, perfect for Arduino use. This may also be known as a “potentiometer ”.

<p style="text-align:center"><a href="https://www.seeedstudio.com/Grove-Rotary-Angle-Sensor-p-770.html" target="_blank"><img src="https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/get_one_now_small.png" width="200" height="38"  border=0 /></a></p>

There is another product, Grove - Rotary Angle Sensor(P). What does “P” mean? “P” is for “panel mount” in this product.It is the sister version of Grove - Rotary Angle Sensor. They are identical except the Grove connecter is moved to the back so that you can easily use it as a neat and wire-free human interface device.

<table>
    <tr>
        <td>
            <img src="https://raw.githubusercontent.com/SeeedDocument/Grove-Rotary_Angle_Sensor/master/img/Grove-Rotary_Angle_Sensor-P-.jpg">
        </td>
        <td>
            <img src="https://raw.githubusercontent.com/SeeedDocument/Grove-Rotary_Angle_Sensor/master/img/GroveRotaryP_02.jpg">
        </td>
    </tr>
</table>

<p style="text-align:center"><a href="http://www.seeedstudio.com/depot/grove-rotary-angle-sensorp-p-1242.html" target="_blank"><img src="https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/get_one_now_small.png" width="200" height="38"  border=0 /></a></p>

## Version

| Product Version                   | Changes                              | Released Date |
|-----------------------------------|--------------------------------------|---------------|
|Grove-Rotary Angle Sensor(P) V1.1  | Initial                              | Jan 2013    |   
|Grove-Rotary Angle Sensor V1.2     | Initial                              | May 2014    |    


## Features

-   Grove Interface
-   Easy to Use
-   Grove Base Module

!!!Tip
    More details about Grove modules please refer to [Grove System](http://wiki.seeedstudio.com/Grove_System/)

## Specifications


<table border="1" cellspacing="0" width="80%">
<tr>
<th scope="col">
Item
</th>
<th scope="col">
Min
</th>
<th scope="col">
Typical
</th>
<th scope="col">
Max
</th>
<th scope="col">
Unit
</th>
</tr>
<tr align="center">
<th scope="row">
Voltage
</th>
<td>
4.75
</td>
<td>
5.0
</td>
<td>
5.25
</td>
<td>
VDC
</td>
</tr>
<tr align="center">
<th scope="row">
Rotary Angle
</th>
<td>
0
</td>
<td>
~
</td>
<td>
300
</td>
<td>
Deg
</td>
</tr>
<tr align="center">
<th scope="row">
Dimension
</th>
<td colspan="3">
19x19x30.1
</td>
<td>
mm
</td>
</tr>
</table>

## Platforms Supported

| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo.jpg) |

!!!Caution
    The platforms mentioned above as supported is/are an indication of the module's hardware or theoritical compatibility. We only provide software library or code examples for Arduino platform in most cases. It is not possible to provide software library / demo code for all possible MCU platforms. Hence, users have to write their own software library.

## Getting Started

!!!Note
    If this is the first time you work with Arduino, we firmly recommend you to see [Getting Started with Arduino](http://wiki.seeedstudio.com/Getting_Started_with_Arduino/) before the start.


### Play With Arduino

**Hardware**

- **Step 1.** Prepare the below stuffs:

| Seeeduino V4.2 | Base Shield|  Grove-Rotary Angle Sensor |Grove-LED|
|--------------|-------------|-----------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/seeeduino_v4.2.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/base_shield.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Rotary_Angle_Sensor/raw/master/img/rorary_s.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Rotary_Angle_Sensor/raw/master/img/grove_led.jpg)|
|[Get One Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get One Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get One Now](https://www.seeedstudio.com/Grove-Rotary-Angle-Sensor-p-770.html)|[Get One Now](https://www.seeedstudio.com/Grove-LED-p-767.html)|

- **Step 2.** Connect Grove-Rotary Angle Sensor to **A0** port of Grove-Base Shield.
- **Step 3.** Connect Grove-LED to **D3** port of Grove-Base Shield. 
- **Step 4.** Plug Grove - Base Shield into Seeeduino.
- **Step 5.** Connect Seeeduino to PC via a USB cable.

![](https://github.com/SeeedDocument/Grove-Rotary_Angle_Sensor/raw/master/img/seeeduino_rotary.jpg)

!!!Note
	If we don't have Grove Base Shield, We also can directly connect Grove-Rotary Angle Sensor and Grove-Led to Seeeduino as below. Grove-Led must be connected to PWM port. For Seeeduino, they are D3,5,6,9,10,11. 

| Seeeduino | Grove-Rotary Angle Sensor | Seeeduino | Grove-LED |
|-----------|---------------------------|-----------|-----------|
| 5V        | Red                       | 5V        | Red       |
| GND       | Black                     | GND       | Black     |
| NC        | White                     | NC        | White     |
| A0        | Yellow                    | D3        | Yellow    |

**Software**

- **Step 1.** Please copy below code to Arduio IDE and upload to arduino. If you do not know how to upload the code, please check [how to upload code](http://wiki.seeedstudio.com/Upload_Code/).


```c++
/*macro definitions of Rotary angle sensor and LED pin*/

#define ROTARY_ANGLE_SENSOR A0
#define LED 3  //the Grove - LED is connected to PWM pin D3 of Arduino
#define ADC_REF 5 //reference voltage of ADC is 5v.If the Vcc switch on the seeeduino
                    //board switches to 3V3, the ADC_REF should be 3.3
#define GROVE_VCC 5 //VCC of the grove interface is normally 5v
#define FULL_ANGLE 300 //full value of the rotary angle is 300 degrees

void setup()
{
    Serial.begin(9600);
    pinMode(ROTARY_ANGLE_SENSOR, INPUT);
    pinMode(LED,OUTPUT);   
}

void loop()
{   
    float voltage;
    int sensor_value = analogRead(ROTARY_ANGLE_SENSOR);
    voltage = (float)sensor_value*ADC_REF/1023;
    float degrees = (voltage*FULL_ANGLE)/GROVE_VCC;
    Serial.println("The angle between the mark and the starting position:");
    Serial.println(degrees);

    int brightness;
    brightness = map(degrees, 0, FULL_ANGLE, 0, 255);
    analogWrite(LED,brightness);
    delay(500);
}

```

- **Step 2.** Adjust Grove-Rotary Angle Sensor and we will see the Grove-LED changes the brightness.


### Play With Raspberry Pi

**Hardware**

- **Step 1.** Prepare the below stuffs:

| Raspberry pi | GrovePi_Plus |  Grove-Rotary Angle Sensor |Grove-LED|
|--------------|-------------|-----------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/Grovepi%2B.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Rotary_Angle_Sensor/raw/master/img/rorary_s.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove-Rotary_Angle_Sensor/raw/master/img/grove_led.jpg)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/GrovePi%2B-p-2241.html)|[Get One Now](https://www.seeedstudio.com/Grove-Rotary-Angle-Sensor-p-770.html)|[Get One Now](https://www.seeedstudio.com/Grove-LED-p-767.html)|


- **Step 2.** Plug the GrovePi_Plus into Raspberry.
- **Step 3.** Connect Grove-Rotary Angle Sensor to **A0** port of GrovePi_Plus.
- **Step 4.** Connect Grove-LED to **D5** port of GrovePi_Plus.
- **Step 5.** Connect the Raspberry to PC through USB cable.

![](https://github.com/SeeedDocument/Grove-Rotary_Angle_Sensor/raw/master/img/rpi_rotary.jpg)

**Software**

- **Step 1.** Follow [Setting Software](https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/setting-software/) to configure the development environment.
- **Step 2.** Git clone the Github repository.

```
cd ~
git clone https://github.com/DexterInd/GrovePi.git

```

- **Step 3.** Excute below commands to monitor the loudness.


```python
cd ~/GrovePi/Software/Python
python grove_rotary_angle_sensor.py
```

Here is the grove_rotary_angle_sensor.py code.

```python
import time
import grovepi

# Connect the Grove Rotary Angle Sensor to analog port A0
# SIG,NC,VCC,GND
potentiometer = 0

# Connect the LED to digital port D5
# SIG,NC,VCC,GND
led = 5

grovepi.pinMode(potentiometer,"INPUT")
grovepi.pinMode(led,"OUTPUT")
time.sleep(1)

# Reference voltage of ADC is 5v
adc_ref = 5

# Vcc of the grove interface is normally 5v
grove_vcc = 5

# Full value of the rotary angle is 300 degrees, as per it's specs (0 to 300)
full_angle = 300

while True:
    try:
        # Read sensor value from potentiometer
        sensor_value = grovepi.analogRead(potentiometer)

        # Calculate voltage
        voltage = round((float)(sensor_value) * adc_ref / 1023, 2)

        # Calculate rotation in degrees (0 to 300)
        degrees = round((voltage * full_angle) / grove_vcc, 2)

        # Calculate LED brightess (0 to 255) from degrees (0 to 300)
        brightness = int(degrees / full_angle * 255)

        # Give PWM output to LED
        grovepi.analogWrite(led,brightness)

        print("sensor_value = %d voltage = %.2f degrees = %.1f brightness = %d" %(sensor_value, voltage, degrees, brightness))
    except KeyboardInterrupt:
        grovepi.analogWrite(led,0)
        break
    except IOError:
        print ("Error")

```

- **Step 4.** Adjust Grove-Rotary Angle Sensor and we will see the Grove-LED changes the brightness.



### Play with TI LaunchPad

**Reading the Potentiometer (Rotary Angle Sensor)**

This example shows how to read the analog output coming from the Grove potentiometer module. We will be combining a few Grove modules in this example! By turning the potentiometer knob, we will display the analog reading value on the Grove 4-digital display.

![](https://raw.githubusercontent.com/SeeedDocument/Grove-Rotary_Angle_Sensor/master/img/Angle_sensor.jpg)

```
/*
    Rotary Angle Sensor
    Demonstrates analog input by reading an analog sensor on J16 of the Grove Base BoosterPack. The speed of the red LED on the LaunchPad will change depending on the position of the potentiometer knob. This example will also display the analog reading value on the Grove 4-digital display.

    The circuit:
    * Potentiometer attached to pin 24 (J6 on Grove Base BoosterPack)
    * center pin of the potentiometer to the analog pin
    * one side pin (either one) to ground
    * the other side pin to VCC (3.3V)

    * Note: Because of unstable of the voltage, the value of the rotary angle sensor
            varies slightly from run to run even you don't touch it.  

    Created by Oliver Wang

    This example code is in the public domain.

    http://www.seeedstudio.com/wiki/GROVE_-_Starter_Kit_v1.1b#Grove_-_Rotary_Angle_Sensor
    */

#include "TM1637.h"

/* Macro Define */
#define CLK               39                  /* 4-digital display clock pin */
#define DIO               38                /* 4-digital display data pin */
#define ROTARY_ANGLE_P    24               /* pin of rotary angle sensor */

/* Global Variables */
TM1637 tm1637(CLK, DIO);                  /* 4-digital display object */
int analog_value = 0;                     /* variable to store the value coming from rotary angle sensor */

int8_t bits[4] = {0};                     /* array to store the single bits of the value */

/* the setup() method runs once, when the sketch starts */
void setup() {

    /* Initialize 4-digital display */
    tm1637.init();
    tm1637.set(BRIGHT_TYPICAL);

}

/* the loop() method runs over and over again */
void loop() {   

    analog_value = analogRead(ROTARY_ANGLE_P);      /* read the value from the sensor */
    memset(bits, 0, 4);                             /* reset array when we use it */
    for(int i = 3; i >= 0; i--) {
        /* get single bits of the analog value */
        bits[i] = analog_value % 10;
        analog_value = analog_value / 10;  
        tm1637.display(i, bits[i]);                 /* display by 4-digital display */
    }
    delay(100);
}
```


## Resources

-  **[Eagle&PDF]** [Grove-Rotary Angle Sensor v1.2 Schematic File](https://github.com/SeeedDocument/Grove-Rotary_Angle_Sensor/raw/master/res/Grove%20-%20Rotary%20Angle%20Sensor%20v1.2.zip)
-  **[Eagle&PDF]** [Grove - Rotary Angle Sensor(P) v1.1 Schematic File](https://github.com/SeeedDocument/Grove-Rotary_Angle_Sensor/raw/master/res/Grove%20%20-%20Rotary%20Angle%20Sensor(P)%20v1.1.zip)
-  **[Library]** [Github repository for Rotary Angle Sensor](https://github.com/Seeed-Studio/Grove_Rotary_Angle_Sensor)

## Tech Support
Please do not hesitate to contact [techsupport@seeed.cc](techsupport@seeed.cc) if you have any technical issue. Or submit the issue into our [forum](http://forum.seeedstudio.com/). 