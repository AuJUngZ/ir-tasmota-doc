# What about this project?

This project is a IR remote control for many of Televisions in [TLIC](https://www.info.tlic.cmu.ac.th/) building [Chinag Mai University](https://www.cmu.ac.th/).

### flow control of this project.

1. User touch the screen from Nspanel to select television that they want to control.
2. User can power on/off, change channel, change volume, and mute the television.

> behind the scene, we use ESP32 connect with PCB that have already attached IR LED to send IR signal to television.
> Meanwhile, ESP32 connect to Home Assistant server to get MQTT message that has been sent from Nspanel (Nspanel connect to HASS also).

### Goal of this documentation.
To make developer who come to do this project in the future can understand the flow of this project and can configure it easily by
following this documentation.

>Get started with this project by click [here](/docs/tasmota-config.md)