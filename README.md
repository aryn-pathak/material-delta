# MATERIAL DELTA (stylised as mδ)
## Concept:
**"What if a printer was 3D printed?"** _thats called a reprap printer, nothing new, duh!_

**"Alright, what if it was super cheap, about $150?"** _Impressive, but it's probably super small, super slow, and super low quality too. why not splurge the $350 limit you have!_

**"Nope, what if it was ultra fast too?"** _powerful motors and a 100W hotend, nothing special either-- probably eats up a TON of power!_

**"Can't you ever be happy?! Fine, what if it was powered by USBC?"** _you're kidding thats not possible blah blah blah about how a 3D printer can't be powered by USBC_

The Material DELTA is an opensource delta style 3D printer, built for speed, pockets, and powered by USBC, powered by a RPi Zero 2W running klipper, with raspberry pi pico controlling motors for high speed motion.

## images (they're beautiful)
![pic](https://hc-cdn.hel1.your-objectstorage.com/s/v3/8a4dcad0904abcef704119de1344ff9c21bd588e_img-20250609-wa0000.jpg)

![pic](https://hc-cdn.hel1.your-objectstorage.com/s/v3/85646aa2813d91d2908066b0b6b41089a6ea1d99_img-20250609-wa0001.jpg)

![pic](https://hc-cdn.hel1.your-objectstorage.com/s/v3/7a84de9ee1d1bf4c3e9fcd3e8fa14ff9d337cd1a_img-20250609-wa0002.jpg)

# BOM:


| Category         | Name                               | Link                                                                                                                                                                                                                     | Price (INR) | Price (USD) |
|------------------|------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------|-------------|
| CONTROLLER PARTS | NCE4080K                           | [Link](https://roboticsdna.in/product/nce4080k-40v-80a-n-channel-enhancement-mode-power-mosfet/)                                                                                                                         | 108         | 1.296       |
|                  | PDC004-PD                          | [Link](https://robu.in/product/pdc004-pd-pd-decoy-module-20v/)                                                                                                                                                           | 109         | 1.308       |
|                  | SMBJ6.0A                           | [Link](https://roboticsdna.in/product/smbj6-0a-6v-600w-esd-suppressor-tvs-diode-2pin-smb-do-214aa/)                                                                                                                      | 20          | 0.24        |
|                  | 100uF 25V Electrolytic Capacitor   | [Link](https://robu.in/product/100uf-25v-electrolytic-capacitor-pack-of-10/)                                                                                                                                             | 6           | 0.072       |
|                  | 1N5819                             | [Link](https://roboticsdna.in/product/in5819-schottky-diode/)                                                                                                                                                            | 61          | 0.732       |
|                  | Connector (x2)                     | [Link](https://roboticsdna.in/product/xy2500-9-pin-3-81-mm-male-pitch-straight-screw-terminal-block-socket/)                                                                                                             | 391         | 4.692       |
|                  | Orpheus Pico                       | available @ home                                                                                                                                                                                                         | 0           | 0           |
|                  | RPi Zero 2W                        | available @ home                                                                                                                                                                                                         | 0           | 0           |
|                  | TMC2226 Stepper driver (x4)        | [Link](https://novo3d.in/tmc2226-driver/)                                                                                                                                                                                | 1796        | 21.552      |
|                  | XL4015 Step down                   | [Link](https://robu.in/product/xl4015-5a-dc-dc-step-down-adjustable-power-supply-buck-module-led-with-heatsink/)                                                                                                        | 75          | 0.9         |
|                  | XL6019E1 Step up                   | [Link](https://robu.in/product/xl6019e1-dc-dc-step-converter-performance-ultra-lm2577-booster-circuit-board/)                                                                                                            | 155         | 1.86        |
| PRINTER PARTS    | Nema 17 (x4)                       | [Link](https://novo3d.in/42-stepper-motor-nema17/)                                                                                                                                                                       | 2316        | 27.792      |
|                  | Volcano heatblock                  | [Link](https://novo3d.in/pt100-volcano-heat-block/)                                                                                                                                                                     | 149         | 1.788       |
|                  | Heater                             | [Link](https://novo3d.in/24v-50w-heater-cartridge/)                                                                                                                                                                      | 99          | 1.188       |
|                  | Heatbreak                          | [Link](https://novo3d.in/ender3-s1-sprite-throat/)                                                                                                                                                                      | 169         | 2.028       |
|                  | CHT Nozzle (0.6mm)                 | [Link](https://novo3d.in/v6-cht-nozzle/)                                                                                                                                                                                 | 129         | 1.548       |
|                  | Heatsink                           | [Link](https://novo3d.in/e3d-v6-heatsink/)                                                                                                                                                                               | 79          | 0.948       |
|                  | 3010 Fan                           | [Link](https://robu.in/product/12v-3010-cooling-fan-for-3d-printer/)                                                                                                                                                     | 71          | 0.852       |
|                  | Pneumatic connector                | [Link](https://novo3d.in/pc4-m6/)                                                                                                                                                                                        | 20          | 0.24        |
|                  | Tube (x2)                          | [Link](https://novo3d.in/ptfe-tube-white/)                                                                                                                                                                               | 218         | 2.616       |
|                  | 2020 extrusions (5m)               | [Link](https://www.fastdep.in/product/tslot-2020/?src=search&q=2020)                                                                                                                                                     | 1895        | 22.74       |
|                  | Titan extruder                     | [Link](https://novo3d.in/titan-extruder/)                                                                                                                                                                                | 399         | 4.788       |
|                  | Ball joints for arms               | [Link](https://roboticsdna.in/product/reprap-delta-kossel-mini-5347-delta-ball-headed-buckle-ball-caps-parallel-arm-rod-carbon-rod-joints-kit-with-12pcs-m3-for-3d-printer/)                                           | 400         | 4.8         |
|                  | Carbon fiber arms (x2)             | [Link]([https://robu.in/product/pultruded-carbon-fiber-tube-hollow-3mmod-1-5mm-id-1000mm-pack-of-2/](https://robu.in/product/pultruded-carbon-fiber-tube-hollow-6mm-4mm-500mm-pack-of-2/))                                                                                                                     | 642         | 7.51       |
|                  | GT2 timing pulley (x3)             | [Link](https://novo3d.in/motor-pulley/)                                                                                                                                                                                  | 75          | 0.9         |
|                  | Idler pulley                       | [Link](https://novo3d.in/idler-pulley-6mm/)                                                                                                                                                                              | 65          | 0.78        |
|                  | GT2 timing belt                    | [Link](https://novo3d.in/gt2-6mm-belt/)                                                                                                                                                                                  | 120         | 1.44        |
|                  | V Slot wheels (x9)                 | [Link](https://novo3d.in/v-wheel/)                                                                                                                                                                                       | 1071        | 12.852      |
|                  | 2040 extrusion (3m)                | [Link](https://www.fastdep.in/product/tslot-vslot-2040/?src=search&q=2040%2520extrusions)                                                                                                                               | 2646        | 31.752      |
|                  | 5010 blower                        | [Link](https://novo3d.in/blower-cooling-fan-5015/)                                                                                                                                                                      | 75          | 0.9         |
|                  | Thermistor                         | [Link](https://novo3d.in/ntc-sensor/)                                                                                                                                                                                    | 99          | 1.188       |
|                  | 1kg PLA                            | [Link](https://novo3d.in/filament/)                                                                                                                                                                                      | 799         | 9.588       |
|                  | 10mm Spiral Wrapping               | [Link](https://robu.in/product/10mm-spiral-wrapping-band-black-10m-for-wires/)                                                                                                                                           | 90          | 1.08        |
|                  | Round bed sticker                  | [Link](https://robu.in/product/round-heated-bed-sticker-for-3d-printer-build-plate-with-adhesive-backing/)                                                                                                               | 274         | 3.288       |
|                  | PVC tape                           | [Link](https://robu.in/product/pro-power-pvc-tape-1920b-general-purpose-tape-pvc-20m-x-19mm/)                                                                                                                            | 167         | 2.004       |
|                  | Endstop switches (x6)              | [Link](https://roboticsdna.in/product/omron-3d-printer-limit-switch-endstop-ss-5gl/)                                                                                                                                     | 240         | 2.88        |
| FASTENERS        | M3 x 12mm                          | [Link](https://www.fastdep.in/product/socket-head-m3x12mm/)                                                                                                                                                             | 26          | 0.312       |
|                  | M3 x 25mm (x2)                     | [Link](https://www.fastdep.in/product/socket-head-screws-m3x25mm/)                                                                                                                                                       | 60          | 0.72        |
|                  | M5 x 10mm (x5)                     | [Link](https://www.fastdep.in/product/socket-head-screws-m5x10mm/)                                                                                                                                                       | 140         | 1.68        |
|                  | M3 Hex Nut                         | [Link](https://www.fastdep.in/product/hex-nut-m3/)                                                                                                                                                                       | 18          | 0.216       |
|                  | M5 hammernut (x50)                 | [Link](https://novo3d.in/hammernut/)                                                                                                                                                                                     | 300         | 3.6         |
|                  | M2.5 x 8mm                         | [Link](https://www.fastdep.in/product/pan-head-screw-m2-5x8mm/)                                                                                                                                                          | 48          | 0.576       |
| **TOTAL**        |                                    |                                                                                                                                                                                                                          | **₹15500**  | **$186**    |


Huge huge huge thanks to Hack Club and for making this possible :D

# EDITS AFTER SUBMISSION 

- Made new duct, with clearance and pointing right below the nozzle (instead of on it)

![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/6fbb0ac63ad86bbb9453cc5bbdc26b4ebe4439bd_img_0437.jpg)

- Made it taller for more Z axis
- Added bowden mount for extruder
- Added filament holder

![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/e9eb9c6ef11d5682f2b4bb4cda2585be4231fcbc_img_0439.jpg)

- Modelled in the boards

![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/6a45768d1c6a08bc33399e1b9a9c553a3f4d5050_img_0438.jpg)

# MORE EDITS AFTER SUBMISSION
- Fixed duct based on feedback from reviewers!
![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/f2c3d4b18db15aea9853139488581173a05e6f26_img_0442.jpg)

- Made new filament holder
![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/930c8f842899a17eacacc1dce9ec01015286f33e_img_0443.jpg)

- Added belt tensioners!
![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/ee7d6f2020f1d97f607929e51035c1a083495c4f_img_0441.jpg)
