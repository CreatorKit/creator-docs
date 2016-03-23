![Creator Logo](../images/creatorlogo.png)

# Project 1 - IoT Button

## Introduction

This project will allow you to press a button on one of your Clicker boards and see an LED toggle on the other Clicker board. Ci40 acts as the hub for the 6LoWPAN communication. You can also view the inter-device messages via the FlowM2M website - demonstrating connectivity with the cloud.

This project requires the Ci40 and 2 Clicker boards from Creator Kit. It does not require any of the 3 Click expansion boards.

## Steps

To complete these steps, refer to the [Toolbox](Toolbox.md) for detailed descriptions of each action. You will need a [FlowM2M account](Toolbox.md#creating-a-flowm2m-account) too.

* Get the code: [Pre-built Release](http://github.com/creatorkit) or [Source Code](http://github.com/creatorkit)
* [Flash](Toolbox.md#programming-a-6lowpan-clicker) the ""lwm2m-client-contiki-button"" hex file onto one Clicker board - Make a note of which one it is
* [Flash](Toolbox.md#programming-a-6lowpan-clicker) the ""lwm2m-client-contiki-led"" hex file onto the second Clicker board - Make a note of which one it is
* [Connect](Toolbox.md#connecting-ci40-to-the-internet) Ci40 to the Internet
* [Provision](Toolbox.md#provisioning-ci40) Ci40
* Power on both Clicker boards
* [Provision](Toolbox.md#provisioning-clicker) the Clickers via the Ci40 web interface
* Press the button on the Button Clicker and observe the LED on the LED Clicker
* Log into your FlowM2M account and navigate to the Message Viewer - Observe it when you press the Button

## What's next?

We highly recommend you start by doing the first 2 points below. This will aid you in building your own projects and making the most of your Creator Kit.

* Check the "How it works" section below for a high level summary of how this project works
* Download the source code for this project to learn more about how it works, and even edit it to build your own project
* Move on to one of the other example projects in Creator Kit

## How it works

The Ci40 is the hub and gateway of this project. It connects to the Internet (over Ethernet) and to the 2 Clickers (over 6LoWPAN).

The application running on Ci40 allows the Clickers to communicate with each other as well as allowing them to communicate with the cloud.

This functionality can be expanded dramatically (and it is expanded in the other example projects) to make use of the full range of Ci40 features and also get full value from FlowM2M services.
