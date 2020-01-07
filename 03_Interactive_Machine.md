Chapter 3: Interactive Machine and Sensor? / Interactive Machine & Sensitive? Sensor (Electronic Engineer)

Different from the previous visualization chapter and artificial intelligence chapter (which are both belong to computer science area), this chapter will talked about machine and robots in the physical world (which is in the field of Electronic Engineer), in human scale space and how they be responsive to people and environment. In my childhood, every kid dream is having a robots, like bianxingjingang. They are powerful, they have intelligence and assertive. However, these robots are only in the movie of fiction. The robots we can see or have heard are the robots that could listen and speak to you, could clean your room, cook meal, or large manufacturing robots that repeating missions and producing products. In another word, the temporary world is build on the machines. They are almost everywhere in our life.

In landscape architecture, machine could be a great element/system that revitalize/activate the space since machine has huge amount of energy and specific functions. The most common examples are the water features, light features, mechanical/interactive installations. Comparing to the traditional landscape elements like pavement, topography, plants, the elements powered by machine are more energetic, moving , living instead of static, stable, and died. Especially after introducing sensors and program into machine, it becomes much more responsive and interactive to the environment and people. 

As a landscape architect, understanding how these machine work and what these interactive machine could do is essential to communicate with subconsultant, create confident design, or even design and build the specific machine by landscape designer.

3.1.1 Introduction of Single-Board Microcontroller

What is single-board microcontroller? An single-board microcontroller is a microcontroller built onto a single printed circuit board. Basically, it is a mini computer that can store and reading codes, and operate according to the code. It can hook up the machine as out put, sensor or switch as input. Then the program designer will code the program, write into the board. According to the programming code designer converting in, the single-board microcontroller will add input signal(from sensor or switch) as parameter to the program then output some signal to control how the machine move or work. It is principle just like the graph showing below:

3.1.2 The most popular open-source single-board microcontrollers in the market and tech field are Arduino and Raspberry Pi. Followings are brief introductions to these products:

Arduino: Arduino is an open-source electronics platform based on easy-to-use hardware and software. Arduino boards are able to read inputs - light on a sensor, a finger on a button, or a Twitter message - and turn it  into an output - activating a motor, turning on an LED, publishing something online. You can tell your board what to do by sending a set of instructions to the microcontroller on the board. To do so you use the Arduino programming language (based on Wiring), and the Arduino Software (IDE), based on Processing. ... ... ...(https://www.arduino.cc/en/guide/introduction)

Raspberry Pi: The Raspberry Pi is a low cost, credit-card sized computer that plugs into a computer monitor or TV, and uses a standard keyboard and mouse. It is a capable little device that enables people of all ages to explore computing, and to learn how to program in languages like Scratch and Python. It’s capable of doing everything you’d expect a desktop computer to do, from browsing the internet and playing high-definition video, to making spreadsheets, word-processing, and playing games. ([https://www.raspberrypi.org/help/what-%20is-a-raspberry-pi/](https://www.raspberrypi.org/help/what- is-a-raspberry-pi/))

Arduino vs. Raspberry Pi

https://makezine.com/2015/12/04/admittedly-simplistic-guide-raspberry-pi-vs-arduino/



3.1.3 Sensors

Sensor: A sensor is a device that detects and responds to some type of input from the physical environment. The specific input could be light, heat, motion, moisture, pressure, or any one of a great number of other environmental phenomena. The output is generally a signal that is converted to human-readable display at the sensor location or transmitted electronically over a network for reading or further processing. (https://whatis.techtarget.com/definition/sensor)

There are hundreds of different sensors we could use as input signal of the microcontroller. The most common sensor we use includes: 

(https://www.electronicshub.org/different-types-sensors/)

Infrared (IR) Sensor: receive the signals sent from the IR remote controllers.

![IR Sensor](https://hackster.imgix.net/uploads/attachments/471152/obstacle-avoidance-tracking-infrared-sensor-module_S9CxCA7UqZ.jpg?auto=compress&w=900&h=675&fit=min&fm=jpg)

Ultrasonic Distance Sensor: emit a high frequency ultrasonic pulse that bounces back to the onboard ultrasonic sensor. The time delay can be used to determine distances surprisingly accurate.

![Ultrasonic Distance Sensor](https://cdn.sparkfun.com//assets/parts/1/3/5/0/8/15569-Ultrasonic_Distance_Sensor_-_HC-SR04-01a.jpg)

Soil Moisture Sensor: The Soil Moisture Sensor uses capacitance to measure the water content of soil (by measuring the dielectric permittivity of the soil, which is a function of the water content). Simply insert this rugged sensor into the soil to be tested, and the volumetric water content of the soil is reported in percent.

![Soil Moisture Sensor](https://media.ncd.io/sites/2/20180301093006/ADC121C021-SMS-I2CS_1.png)

Temperature Sensor: Temperature Sensors measure the amount of heat energy or even coldness that is generated by an object or system, allowing us to “sense” or detect any physical change to that temperature producing either an analogue or digital output.

![Temperature Sensor](https://www.electronics-tutorials.ws/wp-content/uploads/2018/05/io-io55a.jpg)



Metal Touch/Human Touch Sensor:

![TouchSensor](https://imgaz.staticbg.com/thumb/large/upload/2012/lidanpo/SKU117322%20(1).jpg)

Vibration Sensor:

![Vibration Sensor](https://images-na.ssl-images-amazon.com/images/I/61lsguaHTiL._SL1100_.jpg)

Proximity Sensor: ![Proximity Sensor](https://www.ato.com/content/images/thumbs/0000925_proximity-sensor-capacitive-m12-pnp_550.jpeg)

Accelerometer Module: 

![Accelerometer Sensor](https://www.smart-prototyping.com/image/cache/data/SKU%20Photos/10100071/DSC_0281-750x750.JPG)

Pyroelectric Infrared Sensor:

![Pyroelectric Infrared Sensor](https://image.made-in-china.com/202f0j00itMYQmlIVgcT/Cheap-PIR500bp-Pyroelectric-Infrared-PIR-Sensor-for-Light-Dependent-Control-Light.jpg)



3.2 Application of Single-Board Microcontroller in Design Fields

3.2.1 Light and LED Installation  **All the video materials are available on [[aodabo.tech]](aodabo.tech))

-  LED Table Light(http://cdn.designrulz.com/wp-content/uploads/2012/06/led-outdoor-lighting-fixtures-halley-vibia-00.jpg)
- LED Highlight(http://www.litecraft.co.uk/blog/wp-content/uploads/2014/06/crazy-LED-eyelashes-537x399.jpg)
- Eric and Deborah Staller Bubble Heads(https://abc.nl/blog/wp-content/uploads/2009/03/bubbleheads.jpg)
- Aqua Teen Hunger Force - 2007 Boston Mooninite (https://en.wikipedia.org/wiki/2007_Boston_Mooninite_panic)
- Bay Bridge LED (https://www.youtube.com/watch?v=HxYeZ9GOdpQ)
- Leo Villareal compliation (https://vimeo.com/121570561)
- Collectif Coin (https://vimeo.com/78616683)
- Listening Post Video by Mark Hansen and Ben Rubin(http://vimeo.com/3885443)
- Elliott Malkin's laser eruv(http://dziga.com/laser/)
- Jim Campbell(http://www.fondation-langlois.org/e-art/e/jim-campbell.html)
- Peter Vogel(http://www.bitforms.com/peter-vogel.html#id=7&num=4)
- Leo Villareal (https://www.youtube.com/watch?v=mRwey_tqfVI)
- May search more from the Youtube

3.2.2 Sound Installation

- Nina Katchadourian(http://www.ninakatchadourian.com/languagetranslation/accent.php)
- Natural Car Alarms(http://www.ninakatchadourian.com/confusinganimals/caralarms.php)
- 

3.2.3 Water Feature Programming

3.2.4 Interactive Art

- Artwork inspired by migraines(https://www.youtube.com/watch?v=4apVW2wD2pY)
- Daniel Jolliffe Perfect View(http://www.danieljolliffe.ca/pv/pv.htm)
- Daniel Jolliffe One Free Minute video(http://www.danieljolliffe.ca/ofm/ofm.htm)

3.2.5 Other Examples



3.3 Simple Guide to the Single-Board Microcontroller

3.3.1 Programming a LED light

Preparation:

Devices: Arduino Uno Board, Breadboard, LED light bulb, usb cable, resistors

Software: Arduino IDE

Step 1: Wire your devices as the image showing

Step 2: Open the Arduino IDE and connect Uno board to your computer

Step 3: Open example code, and upload to the board

Step 4: Alter the default code, make your own program



3.3.2 Build an interactive installation - Sensorial Lamp

After completion of the simple exercise, you start to know how it works from code / programming to machine / movement. Next step,try using your imagination as a designer to create an interactive installation. This tutorial will teach you to create a responsive machine by using sensors.













