# Scope

Creator Kit has been designed to be the building blocks of your IoT solution. Ci40 is the hub and gateway, Clicker boards offer remote sensors and actuators, and FlowM2M services allow data to be sent, stored and visualized.

The kit itself has 5 example projects which are detailed in this guide. Setting them up is easy, and will give you a working IoT system. These examples are open source and therefore useful not only as a learning resource, but also as the starting point for your own project. This covers embedded software for Ci40 and Clicker boards, as well as iOS/Android apps, and FlowM2M services like LWM2M messaging.

## The Example Projects

#### Project 1 - IoT Button
[Click here to view the project page](Project 1.md)

The first project will allow you to press a button on one Clicker board and turn on an LED on the other. This establishes the basics of communication between your devices. Ci40 acts as the hub for this communication and also ensures that messages are recorded on FlowM2M via the Message Viewer on the FlowM2M website.

After getting this project running, investigating the source code will give you an insight into how to send messages between devices on your network.

#### Project 2 - Motion Controlled Light
[Click here to view the project page](Project 2.md)

Project 2 introduces Click boards to your system. The Motion Click board senses movement in order to simulate an automatic lighting system. Learning how to use the Click interface will allow you to use a huge range of expansion boards to add new sensors and capabilities to your system.

The Creator Kit comes with 3 Click boards used in these projects. You can see a full range of Click boards [here](http://www.mikroe.com/click/)

#### Project 3 - Temperature Logging
[Click here to view the project page](Project 3.md)

This project adds a Thermo3 Click board to the system. This allows you to take data readings from your environment and commit them to a FlowM2M datastore. It also introduces mobile apps (both iOS and Android) for viewing the data in your datastore. Alternatively, this data can be viewed in a browser on you FlowM2M account dashboard. Your datastore can be accessed from anywhere, as long as you have an Internet connection.

#### Project 4 - Remote Relay Control
[Click here to view the project page](Project 4.md)

Project 4 uses a mobile app to control your system remotely. Adding a relay and a control element from the app greatly expands the capabilities of your kit. The Relay Click used in this project is attached to the Ci40 itself rather than a Click board in order to introduce you to the Click interface on Ci40.

#### Project 5 - Automated Climate Control
[Click here to view the project page](Project 5.md)

The final project makes use of most of the features in the earlier projects, but brings it all together into a single system. It does this in a way that also adds automation to some of the processes used in the other projects. You can set thresholds for actuators to respond to, so when temperature reaches a certain point, an actuator will respond. This logic layer dramatically increases the number of potential applications of IoT systems.
