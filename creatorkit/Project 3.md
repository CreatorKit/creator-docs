# Project 3 - Temperature Logging

## Intro

Once set up, this project will sense and store temperature data. A Clicker board with an attached Thermo2 Click board will take temperature readings and send them to the Ci40 gateway. This data will be stored in a FlowM2M datastore so it can be visualised on the web, on an iOS app, or an Android app as long as you have an Internet connection.

This project requires the Ci40 and 1 of the Clicker board from Creator Kit. It also uses one Thermo2 Click board.

## Steps

To complete these steps, refer to the [Toolbox](http://localhost:8000/Toolbox) for detailed descriptions of each action required.

* Get the code: [Pre-built Release](http://github.com) or [Source Code](http://github.com)
* [Flash](http://localhost:8000/Toolbox/#programming-a-6lowpan-clicker) the ""Temperature"" hex file onto one Clicker board and connect the Thermo2 Click board.
* [Connect](http://localhost:8000/Toolbox/#connecting-ci40-to-the-internet) Ci40 to the Internet
* On your Ci40, run the ""command"" command
* [Provision](http://localhost:8000/Toolbox/#provisioning-ci40) Ci40
* Power on both Clicker boards
* [Provision](http://localhost:8000/Toolbox/#provisioning-clicker) the Clickers via the Ci40 web interface
* Log into the FlowM2M website ""Link"" to view the data being collected by your sensor
* Download either the iOS (""Link"") or Android app (""Link"") and login to view the data.


## What's next?

We highly recommend you start by doing the first 2 points below. This will aid you in building your own projects and making the most of your Creator Kit.

* CCheck the "How it works" section below for a high level summary of how this project works
* Download the source code for this project to learn more about how it works, and even edit it to build your own custom project
* Move on to one of the other example projects in Creator Kit

## How it works

The Ci40 is the hub and gateway of this project. It connects to the Internet (over Ethernet) and to the Clicker (over 6LoWPAN).

The Clicker board periodically takes temperature readings from the Thermo2 Click and sends them to the Ci40 gateway (with timestamps). These values are also pushed to a FlowM2M datastore via Ci40. The website and apps read the data from the datastore and display it.
