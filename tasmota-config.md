# Tasmota configuration
> After you install tasmota firmware already, you can config it's following this guide. But if you don't install tasmota firmware yet, you can follow this guide [here](https://tasmota.github.io/docs/).

## Enter tasmota configuration
1. Setup wifi connection for your tasmota device.
2. Open your browser and go to `http://<tasmota-device-ip>`.
3. Click on `Configuration` tab.

## Module configuration
1. Click on `Configure Module` button.
2. Select `ESP32-Devkit(1)` for `Module Type`.
3. Change `GPIO 4` to be `IRsend`. with number `1`.
4. Change `GPIO 18` to be `Led`. with number `1`.
> Notice : `GPIO 4` and `GPIO 18` is pin on esp32 board. You can change it to be compatible with your PCB board design.

## MQTT configuration
1. Click on `Configure MQTT` button.
2. Enter your MQTT server information.
3. Click on `Save` button.

## Console configuration.
1. Click on `Console` tab.
2. Change LED status to mode 4 by use this command `LedState 4`.
3. Add group topic by use this command `GroupTopic<0-4> <group-topic>`.
> this group topic related to your Home Assistant configuration. Use when you want to control all device in same action.