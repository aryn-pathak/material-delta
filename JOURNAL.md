Made by: @aryan Repository link: https://github.com/aryn-pathak/material-zero/ 

TOTAL TIME (source screentime): ~36 Hours (and 40 hours on old printer)

---
title: "Material DELTA"
author: "aryan pathak"
description: "A Delta style printer, powered by USB-C"
created_at: "2025-06-02"
---


Massive thanks to Hack Club and Alex for giving me this insane opportunity to build my own 3D printer!

This is Material DELTA, An open source, superfast, super cheap, (most importantly) USBC powered, Delta-style 3D printer.

## DAY ONE
My old printer wasn't for a long time since i submitted it on 7th of april, but that gave me time to realise that it wasn't good. It was unnecesarily expensive, structure was unstable and probably slow, the printer was very average and didn't have any big innovative feature (just hands free printing powered by an RPi and a web server)
Post some research, I came across a much more uncommon kinematic of 3D printers-- Delta. One of the goals of my old printer (that I realised was beyond unrealistic), was powering it with USBC. A delta printer meant there would be so little load on each motor, current draw would be very minimal.

This is what my old printer design looked like:
![Old printer](https://github.com/user-attachments/assets/cfee9257-4fa6-4e00-8f99-df310d8d2bae)

A solid plan with me, I know I am 100% going to build this.

## DAY TWO - FOUR
I started building the printer. Everything was going very very well. Costs were minimal. I found out that carbon fiber rods were used for the lightweight arms of the printer, but i got a bit carried away, and built the entire printer's frame out of carbon fiber :sob:
I made the carriage too, which would have ball joints (3D printed, and a 8mm ball glued on)

#### CAD and research: ~6 hours

## DAY FIVE-SIX
Wasted a ton of time on making the top and bottom holders (out of carbon fiber too), and with 3D printed holders (very very unstable and inconsistent). Making them took a LOT of time because i was trying to make an equilateral triangle and trying to adjust the rods and the holders and everything, which took 2 days sadly

Corner holders:
![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/46a38859229804d12e5c2d0118798df3440be230_screenshot_20250628-085456.png)
these weren't practical or accurate at all, but this is what it looked like

#### CAD: ~4.5-5 hours

## DAY SEVEN-EIGHT
Did some chatGPT-ing for design ideas, and also realised carbon fiber rods were insanely impractical and unstable, so i decided to make the frame out of 2020 AND 2040 extrusions. Also found something called "Kossel-style corners" which are 3D printed holders for the frame
![kossel corners](https://hc-cdn.hel1.your-objectstorage.com/s/v3/8a7604047e90eb4ef0b0df3963680a9203d99c77_img_0406.jpg)
![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/f475f5214940dc7380f694d27d2b6b7d532c8e06_img_0405.jpg)
![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/166e2051e640e8bdc4808fcce23239e446d3f43c_img_0404.jpg)

I also designed the carriage today:
![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/ef8303c50a4711215ca1f171c3fa7ccdd9aba0fc_img_0408.jpg)
![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/8a7604047e90eb4ef0b0df3963680a9203d99c77_img_0406.jpg)

#### CAD, bit of ChatGPT: ~4.5-5 hours

## DAY NINE
EXTRUDER SHOPPING !! im using a bowden setup, and all hotends are either more expensive than my entire printer or slow and generic. My custom hotend assembly would be made of a V6 heatsink, 65W heat cartridge (not the best, ik, but it fits in my power budget of 100W for USBC), a volcano style heatblock, CHT 0.4mm nozzle, and a bimetal heatbreak.

Volcano heatblock (slightly different from V6, provides better heat retention (needed for low wattage heater):

![Screenshot 2025-06-28 at 4 14 47 PM](https://github.com/user-attachments/assets/d5832562-6553-4279-9ab4-93b98a9eafd1)

CHT nozzle with 3 holes for better melting efficiency:

![Screenshot 2025-06-28 at 4 18 40 PM](https://github.com/user-attachments/assets/7d97036f-7f84-475a-bb57-4e15fd1c525d)

#### Shopping and research: ~2.5-3 hours

## DAY TEN
Curated the BOM, currently, the printer costs about 100USD (1/3rd of the max budget). (remind me to keep making the BOM alongside the printer design process :sob:). Also, i've decided that for the printer, I won't be using a motherboard, but use an RPi Zero (which i have at home) giving it wireless capabilities, running Klipper. But a bit of research revealed that it's GPIO isn't fast enough, and thankfully I also had an orph Pico from highseas lying around, which is much more suitable for swiftly controlling motors.

#### MORE RESEARCH: ~2 hours

## DAY ELEVEN-FOURTEEN
Wasted a ton of time again, this time for designing the effector (the hotend carrier). I had to design a duct for the 5015 blower too, and made 3-4 iterations of it, but finally settled on a super simple duct and overall design, and also looks great.
I even found a set of 12 threaded balls and sockets (called 5347 rod ends), which was really helpful since the 3D printed ones wouldnt give a lot of freedom of movement.
![Screenshot 2025-06-28 at 4 20 42 PM](https://github.com/user-attachments/assets/507b3bdf-74cb-45fe-9db7-881fd83b56eb)

I also found out that these are for 3mm rods, so i had to design an adapter for my 6mm rods:
![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/e49f08b74417b5816ad6a0c806ddaac74bfa6177_img_0409.jpg)

#### mostly CAD: ~9.5-10 hours

## DAY FIFTEEN
I'll try to submit the printer finally today, so the documentation, logs, final BOM, including the most important parts-- USBC PD negotiation board and all the small parts needed to make it work, like buck converters, boosters, etc. finishing touches-- I'll get all that done today and submit it :D

This is a USB-C-PD Decoy board, which negotiates PD (upto 100W) with the power source.
![Screenshot 2025-06-28 at 4 46 29 PM](https://github.com/user-attachments/assets/6af279ec-269a-4f9d-82ea-cc379ece18f1)

## DAY SIXTEEN-SEVENTEEN
Worked on BOM, finishing touches here and there, and finally submitting it after 40+36 hours 😭

#### finishing touches, research, shopping: ~2.5-3 hours

here are some images for you :)
![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/8a4dcad0904abcef704119de1344ff9c21bd588e_img-20250609-wa0000.jpg)
![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/85646aa2813d91d2908066b0b6b41089a6ea1d99_img-20250609-wa0001.jpg)
![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/7a84de9ee1d1bf4c3e9fcd3e8fa14ff9d337cd1a_img-20250609-wa0002.jpg)


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

## NOTE: Aluminium print bed is fixed to extrusions using screws. Will be sut and drilled at a local shop


# EDITS AFTER SUBMISSION 

- Made new duct, with clearance and pointing right below the nozzle (instead of on it)

![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/6fbb0ac63ad86bbb9453cc5bbdc26b4ebe4439bd_img_0437.jpg)

- Made it taller for more Z axis
- Added bowden mount for extruder
- Added filament holder

![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/e9eb9c6ef11d5682f2b4bb4cda2585be4231fcbc_img_0439.jpg)

- Modelled in the boards

![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/6a45768d1c6a08bc33399e1b9a9c553a3f4d5050_img_0438.jpg)