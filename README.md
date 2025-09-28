# Danfoss Ally Home Assistant automations & scripts
Danfoss Ally eTRV automations and scripts for Home Assistant using [Zigbee2MQTT](https://www.zigbee2mqtt.io/). Tested to work with firmware v1.28(00.28.0008 00.28).

### Updating
The blueprints can be updated by importing them again and overwriting the existing one. 

### Breaking changes
Major version number (=v1.x.x) will be updated if any breaking changes are implemented. In this case your existing script might not have input values in correct format. It is recommended to remove any existing input values in YAML editing view if updating to a new major version.

# Weekly schedule scripts
**Note!** The weekly schedule is lost after power cycle or OTA or error state.

### Get weekly schedule
Get weekly schedule from a Danfoss Ally eTRV device. Sends a persistent notification with all schedule transitions for the selected day.

[PLACEHOLDER for import link]

### Set weekly schedule
Set weekly schedule to a Danfoss Ally eTRV device for the selected days.

[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fussaka%2FDanfoss-Ally-HA-automations%2Freleases%2Fdownload%2Fset-schedule-v2.0.0%2Fdanfoss_ally_set_schedule.yaml)

### Clear weekly schedule
Clear weekly schedule from Danfoss Ally eTRV device for all the days.

[PLACEHOLDER for import link]

# External temperature sensor automation
[Blueprint](https://community.home-assistant.io/t/zigbee2mqtt-danfoss-ally-send-external-temperature-to-trv-version-2/627564/8)

### Radiator covered = false
Automatically adjust eTRV's own temperature with offset. The external temperature needs to be send at least every 3 hours but no more often than every 30 minutes @ every 0,1K change.

### Radiator covered = true
Rely only for the external temperature. The external temperature needs to be send at least every 30 minutes but no more often than every 5 minutes @ every 0,1K change.

# ~~Time updater automation~~
<details>
  <summary>Expand</summary>

⚠️ Depracated, see https://github.com/ussaka/Danfoss-Ally-HA-automations/discussions/12 ⚠️

![version](https://img.shields.io/badge/version-1.2.2-blue?style=plastic)

Danfoss Ally has no knowledge of the current time. Zigbee coordinator must send the current time to it. Recommended time update is on weekly interval.

### Note!
- The script will automatically set DST helpers to last sunday of the current year and the helper's month. Please raise an issue if this is a problem for you.

[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fussaka%2FDanfoss-Ally-HA-automations%2Freleases%2Fdownload%2Ftime-updater-v1.2.2%2Fdanfoss_ally_time_updater.yaml)

</details>
