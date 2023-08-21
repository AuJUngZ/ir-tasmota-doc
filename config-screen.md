# This part will not show how to config NsPanel screen.
If you want to learn how to config let's click [here](https://docs.nspanel.pky.eu/).

# Example code of NasPanel screen config
```yaml
--- appdaemon/apps/apps.yaml
nspanel-1:
  module: nspanel-lovelace-ui
  class: NsPanelLovelaceUIManager
  config:
    panelRecvTopic: "tele/{nspanel_topic}/RESULT" //need to change
    panelSendTopic: "cmnd/{nspanel_topic}/CustomSend" //need to change
    model: us-l
    sleepTimeout: 20
    sleepBrightness:
      - time: "sunrise"
        value: 20
      - time: "sunset"
        value: 0
    locale: "en_US"
    screensaver:
      entity: weather.forecast_tlic_cmu_building_1
      theme:
        time: [255, 255, 255]
        date: [93, 173, 226]
        bar: [46, 204, 113]
    cards:
      - type: cardGrid
        title: TLIC A1 ALL
        entities:
          - entity: button.tlic_lg_all_power
            name: Tv Power
            icon: mdi:power
            color: [255, 0, 0]
          - entity: button.tlic_lg_all_vol_up
            name: Vol_up
            icon: mdi:volume-plus
            color: [255, 255, 255]
          - entity: button.tlic_lg_all_vol_down
            name: Vol_down
            icon: mdi:volume-minus
            color: [255, 255, 255]
          - entity: button.tlic_lg_all_mute
            name: Mute
            icon: mdi:volume-off
            color: [255, 255, 255]
          - entity: button.tlic_lg_all_hdmi1
            name: HDMI1
            icon: mdi:television-classic
            color: [255, 255, 255]
      - type: cardGrid
        title: TLIC A1 LG-1
        entities:
          - entity: button.tlic_lg_1_power
            name: Power
            icon: mdi:power
            color: [255, 0, 0]
          - entity: button.tlic_lg_1_vol_up
            name: Vol_up
            icon: mdi:volume-plus
            color: [255, 255, 255]
          - entity: button.tlic_lg_1_vol_down
            name: Vol_down
            icon: mdi:volume-minus
            color: [255, 255, 255]
          - entity: button.tlic_lg_1_mute
            name: Mute
            icon: mdi:volume-off
            color: [255, 255, 255]
          - entity: button.tlic_lg_1_hdmi1
            name: HDMI1
            icon: mdi:television-classic
            color: [255, 255, 255]
      - type: cardGrid
        title: TLIC A1 LG-2
        entities:
          - entity: button.tlic_lg_2_power
            name: Power
            icon: mdi:power
            color: [255, 0, 0]
          - entity: button.tlic_lg_2_vol_up
            name: Vol_up
            icon: mdi:volume-plus
            color: [255, 255, 255]
          - entity: button.tlic_lg_2_vol_down
            name: Vol_down
            icon: mdi:volume-minus
            color: [255, 255, 255]
          - entity: button.tlic_lg_2_mute
            name: Mute
            icon: mdi:volume-off
            color: [255, 255, 255]
          - entity: button.tlic_lg_2_hdmi1
            name: HDMI1
            icon: mdi:television-classic
            color: [255, 255, 255]
      - type: cardGrid
        title: TLIC A1 LG-3
        entities:
          - entity: button.tlic_lg_3_power
            name: Power
            icon: mdi:power
            color: [255, 0, 0]
          - entity: button.tlic_lg_3_vol_up
            name: Vol_up
            icon: mdi:volume-plus
            color: [255, 255, 255]
          - entity: button.tlic_lg_3_vol_down
            name: Vol_down
            icon: mdi:volume-minus
            color: [255, 255, 255]
          - entity: button.tlic_lg_3_mute
            name: Mute
            icon: mdi:volume-off
            color: [255, 255, 255]
          - entity: button.tlic_lg_3_hdmi1
            name: HDMI1
            icon: mdi:television-classic
            color: [255, 255, 255]
      - type: cardGrid
        title: TLIC A1 LG-4
        entities:
          - entity: button.tlic_lg_4_power
            name: Power
            icon: mdi:power
            color: [255, 0, 0]
          - entity: button.tlic_lg_4_vol_up
            name: Vol_up
            icon: mdi:volume-plus
            color: [255, 255, 255]
          - entity: button.tlic_lg_4_vol_down
            name: Vol_down
            icon: mdi:volume-minus
            color: [255, 255, 255]
          - entity: button.tlic_lg_4_mute
            name: Mute
            icon: mdi:volume-off
            color: [255, 255, 255]
          - entity: button.tlic_lg_4_hdmi1
            name: HDMI1
            icon: mdi:television-classic
            color: [255, 255, 255]
      - type: cardGrid
        title: TLIC A1 LG-5
        entities:
          - entity: button.tlic_lg_5_power
            name: Power
            icon: mdi:power
            color: [255, 0, 0]
          - entity: button.tlic_lg_5_vol_up
            name: Vol_up
            icon: mdi:volume-plus
            color: [255, 255, 255]
          - entity: button.tlic_lg_5_vol_down
            name: Vol_down
            icon: mdi:volume-minus
            color: [255, 255, 255]
          - entity: button.tlic_lg_5_mute
            name: Mute
            icon: mdi:volume-off
            color: [255, 255, 255]
          - entity: button.tlic_lg_5_hdmi1
            name: HDMI1
            icon: mdi:television-classic
            color: [255, 255, 255]
```
> As we tell you button entity will use on this code when you what to show button in NsPanel screen. 