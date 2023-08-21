# How to create mqtt button as Entity in Home Assistant.
> If you read this, you probably already have a working Tasmota for esp32 and NsPanel with Home Assistant. If not, please read [Tasmota for esp32 Config](tasmota-config.md) and [NsPanel and Home Assistance config](https://docs.nspanel.pky.eu/).

## Why we need to create button as Entity in Home Assistant?
Because when yuo want to show button in Nspanel you need to create some button entity in HASS first. Then you can use this entity to show in nsplanel.
> If you want to config nsPanel screen, Click [here]().

## How to create button as Entity in Home Assistant?
1. Go to HASS and click on `Studio Code server` plugin.
2. Click on `configurations.yaml` file.
3. Add this code to `configurations.yaml` file.

```yaml
mqtt:
  - unique_id: tlic_lg_all_power
      name: "tlic_lg_all_power"
      command_topic: "cmnd/room1/irsend"
      payload_press: '{ "Protocol": "NEC", "Bits": 32, "Data": 0x20DF10EF }'
      retain: true
   - other button write the same code but change unique_id, name, command_topic and payload_press
```