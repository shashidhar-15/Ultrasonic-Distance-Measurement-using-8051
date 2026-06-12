# Ultrasonic Distance Measurement Using 8051

A simple embedded systems project that measures the distance of an object using the HC-SR04 ultrasonic sensor and displays the result on a 128x64 OLED display.

This project was developed to explore sensor interfacing, timer-based measurements, and OLED communication using the 8051 microcontroller.

## Features

* Non-contact distance measurement
* Real-time distance display on OLED
* Object detection within a predefined range
* Distance shown in both inches and centimeters
* Implemented using an 8052 microcontroller

## Components Used

* 8051 Development Board
* HC-SR04 Ultrasonic Sensor
* 128x64 OLED Display (I2C)
* Breadboard
* Jumper Wires
* Power Supply

## How It Works

1. The HC-SR04 transmits an ultrasonic pulse.
2. The pulse reflects from a nearby object.
3. The sensor returns an echo signal.
4. The 8051 measures the echo duration using its timer.
5. The measured time is converted into distance.
6. The calculated distance is displayed on the OLED screen.

If no object is detected within the configured range, the display shows a "No Object" message.

## Hardware Setup

Connect the HC-SR04 ultrasonic sensor to the 8052 microcontroller and interface the OLED display through I2C communication lines.

The microcontroller generates the trigger pulse, measures the echo response, calculates the distance, and updates the display continuously.

## Results

The system was able to detect objects reliably and display distance measurements in real time. Repeated tests produced consistent readings with minimal variation.

## Learning Outcomes

Through this project, I gained hands-on experience with:

* 8052 microcontroller programming
* Timer and counter operations
* Ultrasonic sensor interfacing
* I2C communication
* OLED display control
* Embedded system debugging

## Future Improvements

* Temperature compensation for improved accuracy
* Wireless monitoring using ESP32
* Data logging capability
* Multiple sensor support
* Improved enclosure and PCB design
