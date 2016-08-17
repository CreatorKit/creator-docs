![Creator Logo](../images/creatorlogo.png)

# Project 3 - Relay controller

## Introduction

In this project mobile app is used to controll the relay click inserted on Ci40. Ci40 acts as a constrained device that is connected to Creator Device Server in cloud. Mobile app uses device server REST API to update IPSO resource on Ci40. Once Ci40 gets notification about IPSO resource update it changes relay state according to received value and responds with operation status.

## Steps
To complete these steps, refer to the [Getting Started](../GettingStarted.md) for detailed descriptions of each action.

* Get the code: Refer [this](../GettingStarted.md#getting-the-code) if you want to build from source or get pre-built binaries.
* [Boot](../GettingStarted.md#running-ci40-board) OpenWrt on Ci40
* [Connect](../GettingStarted.md#connecting-ci40-to-the-internet) Ci40 to the Internet
* [Make](https://console.creatordev.io/) an Creator Account if You don't have it yet
* [Provision](https://github.com/CreatorKit/relay-gateway#app-provisioning) Ci40 to the Creator Device Server
* Run mobile application ([Android](https://github.com/CreatorKit/mobile_power_switch) or [iOS](https://github.com/CreatorKit/mobile_ios_power_switch)) and log in using Creator Account credentials
* Use mobile application to controll relay state on Ci40

## How it works
The Ci40 acts as a constrained device in this project. It connects to the Internet (over Ethernet and Wi-Fi) and registers as a client to Creator Device Server. It observes IPSO digital output resource and changes relay state when notification is received.

Mobile app controls the IPSO digital output resource. It uses Creator Device Server REST API to change the IPSO resource which is then propagated to app running on Ci40.

This project includes two applications

* [**Relay Gateway**](https://github.com/CreatorKit/relay-gateway): Runs on Ci40 and observes IPSO digital output resource registered by itself. Updates relay state as per the changes received. For more info, read [this](https://github.com/CreatorKit/relay-gateway/blob/master/README.md).
* **Mobile power switch** ([Android](https://github.com/CreatorKit/mobile_power_switch) or [iOS](https://github.com/CreatorKit/mobile_ios_power_switch)): Runs on phone and allows to control relay using switch. For more information please refer to [Android](https://github.com/CreatorKit/motion-sensor/blob/master/README.md) and [iOS]() apps docs.
