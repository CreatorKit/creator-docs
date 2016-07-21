![Creator Logo](../images/creatorlogo.png)

# Project 1 - IoT Button

## Introduction

In this project ci40 will observe the status of the buttons on one clicker board, when a button press LWM2M notification is received it will toggle an LED on the Ci40 board. For each button press the LED will toggle on and off.

This project requires the Ci40 and 1 Clicker board from Creator Kit, no expansion boards.

## Steps
To complete these steps, refer to the [Getting Started](../GettingStarted.md) for detailed descriptions of each action.

* Get the code: Refer [this](../GettingStarted.md#getting-the-code) if you want to build from source or get pre-built binaries.
* [Flash](../GettingStarted.md#programming-a-6lowpan-clicker) the "lwm2m-client-button-sensor" hex file onto one Clicker board - Make a note of which one it is
* [Boot](../GettingStarted.md#running-ci40-board) OpenWrt on Ci40
* [Connect](../GettingStarted.md#connecting-ci40-to-the-internet) Ci40 to the Internet
* Press the button on the Button Clicker and observe the LED on ci40 board

## How it works
The Ci40 is the controller of this project. It connects to the Internet (over Ethernet and Wi-Fi) and to the button Clicker (over 6LoWPAN).

The application running on Ci40 allows the Clicker to communicate with itself using AwaLWM2M.

This project includes two applications
* [Led Controller](https://github.com/CreatorKit/led-controller): Runs on Ci40 and observes any button presses on MikroE board, updates led status as per the changes received. For more info, read [this](https://github.com/CreatorKit/led-controller/blob/master/README.md).
* [Button Sensor](https://github.com/CreatorKit/button-sensor): Runs on Clicker and senses any button presses on clicker board, updates button object for gateway. For more info,read [this](https://github.com/CreatorKit/button-sensor/blob/master/README.md).
