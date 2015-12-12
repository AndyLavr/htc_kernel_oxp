# Kernel for device HTC One X+ (enrc2b) version 3.1.10-7-OXP-Wip adapted for the project CyanogenMod 12.1 (Android 5.1.1 Lollipop).

```
This modification of the kernel includes the latest kernel with support S2W and 2A charger.

```


* Kernel Special Features: 2A Charger support, custom s2w/dt2w
---------------


* For international HTC One X+ running latest sense only. NOT for AT&T!


```
It will switch to 2A when D+ and D- are not shorted on the USB connector. And it will always switch 
to 2A mode when put into the CAR dock.
In 2A mode the USB current limit is set to 2100mA and the Charger Constant Current is set to 1500mA.
The settings can be configured by changing the values in these files located in 
/sys/devices/platform/htc_battery fast_charge (1 enable fast charging, 0 disable 
fast charging, including 2A) ultrafast_charge (1 enable 2A charging, 0 disable 2A charging) 
ultrafast_car (1 set 2A charging when in CAR dock, 0 set 1A charging when in CAR dock) 
The default is 1 for all settings.

Fixed S2W pocket detection causing lockups and S2W/DT2W will not respond when touching / swiping with 
more than one finger.

Tegra NEON support added, and improved how the charger chip is set.

Many thanks XtheOne and to all the great devs of various parts and modules that made this possible.

```

A great app to test the charging current is [Ampere](https://play.google.com/store/apps/details?id=com.gombosdev.ampere "Measure the charging and discharging current of your battery"), get it 
on the play store HERE and set interface to 4 (/sys/class/power_supply/battery/batt_current_now).


Copyright (C) 2015  Andrei Lavreniyuk

Copyright (C) 2015  XtheOne

Copyright (C) 2010, 2015 CyanogenMod

Copyright (C) 1989, 2015 Free Software Foundation, Inc.

Licensed under the GNU GENERAL PUBLIC LICENSE Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at <http://fsf.org/>

