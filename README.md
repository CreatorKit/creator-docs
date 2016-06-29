![Creator Logo](images/creatorlogo.png)
----

## Creator
Creator aims to make development on MIPS platforms as simple and accessible as possible. We offer hardware and software to get started, as well as examples/applications that you can use as a base to build from, or as a demonstrator of what's possible on MIPS based hardware platforms. All the software and examples are open source and available on Github. 

## IoT and LWM2M
Multiple device systems and cloud connectivity are becoming increasingly important in embedded systems. Creator provides the means to securely provision devices online to allow safe communication of your data. We also provide open source SDKs and examples of LWM2M to allow inter-device communication on local networks, and over the Internet.

## CreatorKit Overview
Various terminologies used in CreatorKit project are explained at [Glossary](Glossary.md).

CreatorKit projects provides applications which runs on Ci40 MIPS board running with OpenWrt Linux distribution and also makes use of MikroE boards for wide variety of uses.

#### Repositories Overview
CreatorKit project is spread across couple of organizations :-
* [IMGCreator](https://github.com/IMGCreator/): This includes
    * [Contiki](https://github.com/IMGCreator/contiki): Operating system that runs on MikroE boards.
    * [OpenWrt](https://github.com/IMGCreator/openwrt): Linux distribution that runs on Ci40.
    * [Openwrt Feeds](https://github.com/IMGCreator/openwrt-feeds): Collection on third-party  packages required by Openwrt.
* [CreatorKit](https://github.com/CreatorKit/): This includes
    * [Build](https://github.com/CreatorKit/build): Describes steps for building CreatorKit project.
    * [Manifest](https://github.com/CreatorKit/manifest): Manifest for creating directory structure for CreatorKit project.
    * [OpenWrt CreatorKit Feeds](https://github.com/CreatorKit/openwrt-ckt-feeds): Collection of CreatorKit specific packages for OpenWrt.
    * [Webscripts](https://github.com/CreatorKit/webscripts): Package which provides web interface for provisioning CreatorKit devices. It includes webpages as well as webservices.
    * [Libobjects](https://github.com/CreatorKit/libobjects): Collection of lwm2m and custom ipso objects for Clicker apps.
    * [Button Gateway](https://github.com/CreatorKit/button-gateway): CreatorKit [Project 0](projects/Project_0.md) application for Creator Ci40 platform.
    * [Led Controller](https://github.com/CreatorKit/led-controller): CreatorKit [Project 1](projects/Project_1.md) application for Creator Ci40 platform.
    * [Led Actuator](https://github.com/CreatorKit/led-actuator): MikroE 6loWPAN Clicker based LWM2M client led actuator application.
    * [Button Sensor](https://github.com/CreatorKit/button-sensor): MikroE 6loWPAN Clicker based lwm2m client button sensor application.
    * [Device Manager](https://github.com/CreatorKit/device-manager): Application for provisioning the gateway device and constrained devices.
    * [Creator Docs](https://github.com/CreatorKit/creator-docs): Entry level documentation for CreatorKit project.

## Projects
CreatorKit as of now has following projects :-
* [Project 0](projects/Project_0.md)
* [Project 1](projects/Project_1.md)

## Getting Started
Please refer [Getting Started](GettingStarted.md) guide for detailed steps that describes how to get CreatorKit up and running.

## Contributing
We welcome all contributions to this project and we give credit where it's due. Anything from enhancing functionality to improving documentation and bug reporting - it's all good.

Find out more in the [contributor guide](ContributorGuide.md).

## Credits
We would like to thank all of our current [contributors](CONTRIBUTORS).

## License information
All code and documentation developed by Imagination Technologies Limited is licensed under the [BSD 3-clause license](LICENSE).
