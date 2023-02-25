---
title: Overview
layout: home
---

The Joker is a modified V-Core 3 500 3D printer, originally designed by [Rat Rig]. It utilises a [CoreXY motion system] to allow for increased X and Y movement speeds, and has its print bed on the Z-axis to limit the mass that is being moved in lateral directions. More information on the specifics of the stock V-Core 3 can be found [here].

The printer itself currently utilises [RatOS] (v2 beta) as its firmware. This is a modified version [Klipper] firware customised to allow software updates without overiding printer specific settings. Klipper runs in colaboration with [Moonraker], an API to expose printer settings and information, and [Mainsail], which provides the web based front-end interface.

The printer is utilising a [Raspberry Pi Model B 4GB] in partnership with a [Big Tree Tech Octpus Pro 429] control board. It's important to note that the Octopus 429 is not the preferred control board as it does not currently allow software update via USB connection. If Klipper is updated on the RPi, it must be manually flashed to the Octopus via the SD card.

[Rat Rig]: https://www.ratrig.com
[CoreXY motion system]: https://corexy.com/index.html
[here]: https://v-core.ratrig.com/
[RatOS]: https://rat-os.vercel.app
[Klipper]: https://klipper3d.org
[Moonraker]: https://monraker.readthedocs.io
[Mainsail]: docs.mainsail.xyz
[Raspberry Pi Model B 4GB]: https://www.raspberrypi.com/products/raspberry-pi-4-model-b/
[Big Tree Tech Octpus Pro 429]: https://github.com/bigtreetech/BIGTREETECH-OCTOPUS-V1.0
