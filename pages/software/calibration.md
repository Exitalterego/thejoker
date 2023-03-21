---
layout: home
title: Calibration
parent: Software
nav_order: 1
---

* Initial belt tensioning to allow printer to actually work. When: before starting further calibration steps; after belt replacement; after printer teardown and rebuild
* PID Tuning. Ensure the heaters can accurately and stably reach required temps without excessive oscillations. When: to be done when altering cooling, changing the hotend, adding or removing a silicone sock and whenever the print surface material is changed.
```
PID_CALIBRATE HEATER=extruder TARGET=220
SAVE_CONFIG
PID_CALIBRATE HEATER=heater_beb TARGER=60
SAVE_CONFIG
```
* Extruder calibration. E-steps calculated. When: any time the extruder motor is changed. May also need doing if the e-stepper is changed
* Z-offset. Begin with `PROBE_CALIBRATE` and the "paper test". Follow this with.... When: after a new probe is installed.
* First layer squish. Baby step Z axis until we have a good first and second layer. When: any time the nozzle is replaced, anytime the frame is dismantled and rebuilt, any time a filament is used with significantly different temperature (PLA vs ABS). Note that these events may not end up having too much effect on the first layer quality, but they could so this should be looked at in all cases.
* Baseline print. Benchy and calibration cube. These should highlight potential issues to be looked at with future calibrations.