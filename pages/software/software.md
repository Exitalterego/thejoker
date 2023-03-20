---
title: Software
layout: home
nav_order: 5
has_children: true
---

Initial Printer Comissioning
* Check temps report correctly
* Confirm M112 (emergency stop code) works
* Confirm heaters power on and off correctly
* Verify endstops
* Verify stepper motors using STEPPER_BUZZ
* Verify extruder
* PID calibrate extruder and bed heaters
` PID_CALIBRATE HEATER=extruder TARGET=170
SAVE_CONFIG
PID_CALIBRATE HEATER=heater_bed TARGET=60
SAVE_CONFIG `