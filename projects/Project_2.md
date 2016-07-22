![Creator Logo](../images/creatorlogo.png)

# Project 2 - PIR light controller

## Introduction

In this project when the motion sensor detects movement it will raise the IRQ to the PIC, the PIC updates the corresponding IPSO resource. The Ci40 is already observing the resource therefore the clicker will send a LWM2M notification of a state change. On receipt of the LWM2M message the gateway will turn on the LEDs on the Ci40 for a period of 5 seconds. If further movement is detected within the timeout period then the further notifications need to be sent from the clicker and the timeout will be restarted. The 5 second timeout value will be static.

## Steps
To complete these steps, refer to the [Getting Started](../GettingStarted.md) for detailed descriptions of each action.

* Get the code: Refer [this](../GettingStarted.md#getting-the-code) if you want to build from source or get pre-built binaries.
* [Flash](../GettingStarted.md#programming-a-6lowpan-clicker) the "lwm2m-client-motion-sensor" hex file onto one Clicker board - Make a note of which one it is
* [Boot](../GettingStarted.md#running-ci40-board) OpenWrt on Ci40
* [Connect](../GettingStarted.md#connecting-ci40-to-the-internet) Ci40 to the Internet
* Do movement in front of motion-sensor Clicker and observe the LED on Ci40 board glowing for 5 seconds.

## How it works
The Ci40 is the controller of this project. It connects to the Internet (over Ethernet and Wi-Fi) and to the motion-sensor Clicker (over 6LoWPAN).

The application running on Ci40 allows the Clicker to communicate with itself using AwaLWM2M.

This project includes two applications
* [Motion-Led Controller](https://github.com/CreatorKit/motion-led-controller): Runs on Ci40 and observes motion-sensor resource registered by MikroE board, updates led status as per the changes received. For more info, read [this](https://github.com/CreatorKit/motion-led-controller/blob/master/README.md).
* [Motion Sensor](https://github.com/CreatorKit/motion-sensor): Runs on Clicker and detects any movement in the range of motion-click on clicker board, updates sensor object for gateway. For more info,read [this](https://github.com/CreatorKit/motion-sensor/blob/master/README.md).
