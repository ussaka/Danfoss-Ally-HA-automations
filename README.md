# Danfoss Ally improved Home Assistant integration
Danfoss Ally eTRV automatons and scripts for Home Assistant with Zigbee2MQTT.

# Time updater
Danfoss Ally has no knowledge of the current time. Zigbee coordinator must send the current time to it. Recommended time update interval is weekly.

### Installation
**1. Create helpers**
- Schedule
    - Run weekly
- Date and/or time x2
    - Use date and time
    - Set DST start and end times

[![Open your Home Assistant instance and show your helper entities.](https://my.home-assistant.io/badges/helpers.svg)](https://my.home-assistant.io/redirect/helpers/)

**2. Import blueprint and create the automation**

[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fussaka%2FDanfoss-Ally-HA-integration%2Fblob%2Fmain%2Fautomations%2Fdanfoss_ally_time_updater.yaml)