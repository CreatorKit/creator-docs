# Project 2 - Motion Controlled Light

## Intro

Once set up, one of your Clicker boards will be able to detect movement and the other board will react to this by turning on it's LEDs. After a timeout, the LEDs will turn off again. If movement is repeatedly detected the LEDs will stay lit. This project expands on project one by incorporating a Click board for interacting with the environment.

This project requires the Ci40 and 2 Clicker boards from Creator Kit. It requires the PIR movement sensor Click board.

## Steps

To complete these steps, refer to the [Toolbox](Toolbox.md) for detailed descriptions of each action required.

* Get the code: [Pre-built Release](http://github.com/creatorkit) or [Source Code](http://github.com/creatorkit)
* [Flash](Toolbox.md#programming-a-6lowpan-clicker) the ""Movement Sensor"" hex file onto one Clicker board and connect your PIR Movement Sensor Click board.
* [Flash](Toolbox.md#programming-a-6lowpan-clicker) the ""LED"" hex file onto the second Clicker board
* [Connect](Toolbox.md#connecting-ci40-to-the-internet) Ci40 to the Internet
* On your Ci40, run the ""command"" command
* [Provision](Toolbox.md#provisioning-ci40) Ci40
* Power on both Clicker boards
* [Provision](Toolbox.md#provisioning-clicker) the Clickers via the Ci40 web interface
* Move your hand in front of the PIR Movement Sensor Click
* Observe the LED on the LED Clicker
* Log into your FlowM2M account and navigate to the Message Viewer - Observe it when movement is detected and when the LED timeout occurs

## What's next?

We strongly recommend you start by doing the first 2 points below. This will aid you in building your own projects and making the most of your Creator Kit.

* Check the "How it works" section below for a high level summary of how this project works
* Download the source code for this project to learn more about how it works, and even edit it to build your own project
* Move on to one of the other example projects in Creator Kit

## How it works

The Ci40 is the hub and gateway of this project. It connects to the Internet (over Ethernet) and to the 2 Clickers (over 6LoWPAN).

The application running on Ci40 allows the Clickers to communicate with each other as well as allowing them to communicate with the cloud.
