# luci-app-oled

This is the LuCI app written for openwrt  which supports ssd 1306 0.91' oled display on Raspberry Pi 4/CM4

Change the default i2c interface to `/dev/i2c-1`


## Features
---
### Dispaly Info

**0. Enable**

Enable OLED

**1. Autoswitch**

Since the oled display is so bright at night and you hardly ever look at it, you should be invited to provide a timed on/off function, and after checking autoswitch, you can set the start and end time of the **display**.

**2. Time**

Display time.

**3. IP**

The IP address of the LAN port is displayed, remember that the LAN port must not have the **Bridging** option removed or it will fail. Since `br-lan` is used, as different firmware may swap `eth0` and `eth1`.


**4. CPU Temp**

Displays the CPU temperature.

**5. CPU Freq**

Display real-time CPU frequency.

**6. Network Speed**

Provides a choice of different interfaces, `eth0` and `eth1`, which can be modified by individuals as needed. The base unit of network speed is byte instead of bit, [MB/s, KB/s, B/s] so that the displayed number can be smaller and not too long.


**7. Display Interval**

In order to slow down the light decay of oled, a screen saver service is provided to run the screen saver program at set intervals.
