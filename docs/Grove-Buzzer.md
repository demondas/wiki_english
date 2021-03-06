---
title: Grove - Buzzer
category: Actuator
bzurl: https://www.seeedstudio.com/Grove-Buzzer-p-768.html
oldwikiname: Grove - Buzzer
prodimagename: Grove%20Buzzer.jpg
surveyurl: https://www.surveymonkey.com/r/grove-buzzer
sku: 107020000
---


![](https://github.com/SeeedDocument/Grove_Buzzer/raw/master/images/Grove%20Buzzer.jpg)

The Grove - Buzzer module has a [piezo buzzer](https://en.wikipedia.org/wiki/Buzzer#Piezoelectric) as the main component. The piezo can be connected to digital outputs, and will emit a tone when the output is HIGH. Alternatively, it can be connected to an analog pulse-width modulation output to generate various tones and effects.

[![](https://github.com/SeeedDocument/Grove_Buzzer/raw/master/images/300px-Get_One_Now_Banner.png)](https://www.seeedstudio.com/Grove-Buzzer-p-768.html)

## Version


| Product Version              | Changes                                                                                                                                                                                    | Released Date |
|------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|
| Grove-Buzzer V1.0| Initial                                                                                                                                                                                    | Nov 25 2010      |
| Grove-Buzzer V1.1 | Add S9013 Transistor                                                                                                                                                                                    | May 30 2014      |


## Features

- Easy to use piezoelectric buzzer
- Uses Standard 4-pin Grove Cables to connect to other Grove modules such as - [Grove Power Modules](/Grove/Grove_System/) and Grove - Base Shield

!!!Tip
    More details about Grove modules please refer to [Grove System](http://wiki.seeedstudio.com/Grove_System/)

## Specifications

| Items              | Specification |
|--------------------|---------------|
| Operating Voltage  | 4-8V          |
| Sound Output       | ≥85dB         |
| Resonant Frequency | 2300±300Hz    |

## Platforms Supported


| Arduino                                                                                             | Raspberry Pi                                                                                             | BeagleBone                                                                                      | Wio                                                                                               | LinkIt ONE                                                                                         |
|-----------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|
| ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/arduino_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/raspberry_pi_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/bbg_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/wio_logo.jpg) | ![](https://raw.githubusercontent.com/SeeedDocument/wiki_english/master/docs/images/linkit_logo.jpg) |

!!!Caution
    The platforms mentioned above as supported is/are an indication of the module's hardware or theoritical compatibility. We only provide software library or code examples for Arduino platform in most cases. It is not possible to provide software library / demo code for all possible MCU platforms. Hence, users have to write their own software library.


##  Getting Started

### Play With Arduino

#### Hardware

- Step 1. Prepare the below stuffs:

| Seeeduino V4.2 | Base Shield|  Grove - Buzzer |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/seeeduino_v4.2.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/base_shield.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Buzzer/raw/master/img/buzzer_s.jpg)|
|[Get ONE Now](http://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html)|[Get ONE Now](https://www.seeedstudio.com/Base-Shield-V2-p-1378.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Buzzer-p-768.html)|

- Step 2. Connect Grove-Buzzer to port D6 of Grove-Base Shield.
- Step 3. Plug Grove - Base Shield into Seeeduino.
- Step 4. Connect Seeeduino to PC through a USB cable.

![](https://github.com/SeeedDocument/Grove_Buzzer/raw/master/img/seeeduino_buzzer.jpg)

!!!Note
	If we don't have Grove Base Shield, We also can directly connect Grove-buzzer to Seeeduino as below.

| Seeeduino       | Grove-Buzzer |
|---------------|-------------------------|
| 5V           | Red                     |
| GND           | Black                   |
| Not Conencted | White                   |
| D6            | Yellow                  |

#### Software

- Step 1. Copy the code into Arduino IDE and upload.

```c
void setup()
{
  pinMode(6, OUTPUT);
}

void loop()
{
  digitalWrite(6, HIGH);
  delay(analogRead(0));
  digitalWrite(6, LOW);
  delay(analogRead(0));
}
```

- Step 2. We will hear the buzzer on and off.



### Play With Raspberry Pi

#### Hardware

- Step 1. Prepare the below stuffs:

| Raspberry pi | GrovePi_Plus | Grove - Buzzer |
|--------------|-------------|-----------------|
|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/rasp.jpg)|![enter image description here](https://github.com/SeeedDocument/wiki_english/raw/master/docs/images/Grovepi%2B.jpg)|![enter image description here](https://github.com/SeeedDocument/Grove_Buzzer/raw/master/img/buzzer_s.jpg)|
|[Get ONE Now](https://www.seeedstudio.com/Raspberry-Pi-3-Model-B-p-2625.html)|[Get ONE Now](https://www.seeedstudio.com/GrovePi%2B-p-2241.html)|[Get ONE Now](https://www.seeedstudio.com/Grove-Buzzer-p-768.html)|

- Step 2. Plug the GrovePi_Plus into Raspberry.
- Step 3. Connect Grove-Buzzer to D8 port of GrovePi_Plus.
- Step 4. Connect the Raspberry to PC through USB cable.

![](https://github.com/SeeedDocument/Grove_Buzzer/raw/master/img/rasp_buzzer.jpg)

#### Software

- Step 1. Follow [Setting Software](https://www.dexterindustries.com/GrovePi/get-started-with-the-grovepi/setting-software/) to configure the development environment.
- Step 2. Git clone the Github repository.

```
cd ~
git clone https://github.com/DexterInd/GrovePi.git

```
- Step 3. Excute below commands.

```
cd ~/GrovePi/Software/Python
python grove_buzzer.py
```

Here is the grove_buzzer.py code.

```python
import time
import grovepi

# Connect the Grove Buzzer to digital port D8
# SIG,NC,VCC,GND
buzzer = 8

grovepi.pinMode(buzzer,"OUTPUT")

while True:
    try:
        # Buzz for 1 second
        grovepi.digitalWrite(buzzer,1)
        print ('start')
        time.sleep(1)

        # Stop buzzing for 1 second and repeat
        grovepi.digitalWrite(buzzer,0)
        print ('stop')
        time.sleep(1)

    except KeyboardInterrupt:
        grovepi.digitalWrite(buzzer,0)
        break
    except IOError:
        print ("Error")
```

- Step 4. We will hear the buzzer on and off.

```
pi@raspberrypi:~/GrovePi/Software/Python $ python grove_buzzer.py
start
stop
start
stop
```


### Play With TI LaunchPad

#### Hardware

- This example shows how to use the Grove buzzer module to play melodies. It sends a square wave of the appropriate frequency to the buzzer, generating the corresponding tone.

![](https://github.com/SeeedDocument/Grove_Buzzer/raw/master/images/Buzzer.jpg)

#### Software

```c
/*
  Buzzer
 The example use a buzzer to play melodies. It sends a square wave of the
 appropriate frequency to the buzzer, generating the corresponding tone.

 The circuit:
 * Buzzer attached to pin39 (J14 plug on Grove Base BoosterPack)
 * one side pin (either one) to ground
 * the other side pin to VCC
 * LED anode (long leg) attached to RED_LED
 * LED cathode (short leg) attached to ground

 * Note:
 This example code is in the public domain.

 http://www.seeedstudio.com/wiki/index.php?title=GROVE_-_Starter_Kit_v1.1b#Grove_-_Buzzer

*/

/* Macro Define */
#define BUZZER_PIN               39            /* sig pin of the buzzer */

int length = 15;         /* the number of notes */
char notes[] = "ccggaagffeeddc ";
int beats[] = { 1, 1, 1, 1, 1, 1, 2, 1, 1, 1, 1, 1, 1, 2, 4 };
int tempo = 300;

void setup()
{
    /* set buzzer pin as output */
    pinMode(BUZZER_PIN, OUTPUT);
}

void loop()
{
    for(int i = 0; i < length; i++) {
        if(notes[i] == ' ') {
            delay(beats[i] * tempo);
        } else {
            playNote(notes[i], beats[i] * tempo);
        }
        delay(tempo / 2);    /* delay between notes */
    }

}

/* play tone */
void playTone(int tone, int duration) {
    for (long i = 0; i < duration * 1000L; i += tone * 2) {
        digitalWrite(BUZZER_PIN, HIGH);
        delayMicroseconds(tone);
        digitalWrite(BUZZER_PIN, LOW);
        delayMicroseconds(tone);
    }
}

void playNote(char note, int duration) {
    char names[] = { 'c', 'd', 'e', 'f', 'g', 'a', 'b', 'C' };
    int tones[] = { 1915, 1700, 1519, 1432, 1275, 1136, 1014, 956 };

    // play the tone corresponding to the note name
    for (int i = 0; i < 8; i++) {
        if (names[i] == note) {
            playTone(tones[i], duration);
        }
    }
}
```

## Resources

- **[Eagle&PDF]** [Grove - Buzzer Schematic Files v1.1](https://github.com/SeeedDocument/Grove_Buzzer/raw/master/resources/Grove-Buzzer_V1.1_eagle.zip)
- **[Eagle&PDF]** [Grove - Buzzer Schematic Files v1.0](https://github.com/SeeedDocument/Grove_Buzzer/raw/master/resources/Grove_-_Buzzer_v1.0_Source_File.zip)
- **[DataSheet]** [S9013datasheet](https://github.com/SeeedDocument/Grove_Buzzer/raw/master/resources/S9013.pdf)
- **[More Reading]** [Wooden Laser Gun](http://www.instructables.com/id/DIY-a-Wooden-Laser-Gun-As-a-Xmas-Present-for-Your-/)

![](https://raw.githubusercontent.com/SeeedDocument/Grove_Button/master/img/gun.jpg)

Inspired by OVERWATCH, we have made a very cool Wooden Laser Gun toy for fun these day!

The Wooden Laser Gun and the Gun Target are all based on an Arduino board called Seeeduino Lotus. The laser emitter on the Laser Gun is controlled to fire laser pulse to "activate" the Gun Target. And there are 3 light sensors on the Gun Target to detect the laser pulse. It seems very simple right? If you are interested in our project, please make one for yourself or your child! It's worth to spend one day DIY it as a Xmas present.    

## Tech Support
Please do not hesitate to contact [techsupport@seeed.cc](techsupport@seeed.cc) if you have any technical issue. Or submit the issue into our [forum](http://forum.seeedstudio.com/).
