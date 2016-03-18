# Project 4 - Remote Relay Control

## Intro

Once set up, This project will allow you to toggle relays using a mobile app. The mobile app communicates with the Ci40 via FlowM2M so as long as your mobile device and the Ci40 are on the Internet the relay can be toggled. Note that this will not look very spectacular unless you have something to connect to the Relay Click!

This project requires the Ci40 from Creator Kit. It also uses the Relay Click board connected directly to Ci40.

## Steps

To complete these steps, refer to the [Toolbox](http://localhost:8000/Toolbox) for detailed descriptions of each action required.

* Get the code: [Pre-built Release](http://github.com) or [Source Code](http://github.com)
* Connect the Relay Click board to one of the Ci40 Mikrobus sockets
* [Connect](http://localhost:8000/Toolbox/#connecting-ci40-to-the-internet) Ci40 to the Internet
* On your Ci40, run the ""command"" command
* [Provision](http://localhost:8000/Toolbox/#provisioning-ci40) Ci40
* Download the Android app (""Link"") or iOS app (""Link"").
* ""Tap on 'Toggle relay' in the app""

## What's next?

We highly recommend you start by doing the first 2 points below. This will aid you in building your own projects and making the most of your Creator Kit.

* Check the "How it works" section below for a high level summary of how this project works
* Download the source code for this project to learn more about how it works, and even edit it to build your own project
* Move on to one of the other example projects in Creator Kit

## How it works

Ci40 can interface with the attached Click board, and also take input from FlowM2M (using the app). When the application detects the message from the app, the Relay Click toggles. This is a good example of communication between app and Ci40, as well as between Ci40 and attached Click boards.
