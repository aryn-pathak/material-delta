Made by: @aryan Repository link: https://github.com/aryn-pathak/material-zero/ 

TOTAL TIME (source screentime): ~36 Hours (and 40 hours on old printer)


Massive thanks to Hack Club and Alex for giving me this insane opportunity to build my own 3D printer!

This is Material ZERO (zero for being the zero-th version of a printer that will be heavily modified to make better versions down the line.), An open source, superfast, super cheap, (most importantly) USBC powered, Delta-style 3D printer.
(Daily hours not logged unfortunately)

## DAY ONE // 25TH MAY
My old printer wasn't for a long time since i submitted it on 7th of april, but that gave me time to realise that it wasn't good. It was unnecesarily expensive, structure was unstable and probably slow, the printer was very average and didn't have any big innovative feature (just hands free printing powered by an RPi and a web server)
Post some research, I came across a much more uncommon kinematic of 3D printers-- Delta. One of the goals of my old printer (that I realised was beyond unrealistic), was powering it with USBC. A delta printer meant there would be so little load on each motor, current draw would be very minimal.

This is what my old printer design looked like:
![Old printer](https://github.com/user-attachments/assets/cfee9257-4fa6-4e00-8f99-df310d8d2bae)

A solid plan with me, I know I am 100% going to build this.

## DAY TWO - FOUR
I started building the printer. Everything was going very very well. Costs were minimal. I found out that carbon fiber rods were used for the lightweight arms of the printer, but i got a bit carried away, and built the entire printer's frame out of carbon fiber :sob:
I made the carriage too, which would have ball joints (3D printed, and a 8mm ball glued on)

## DAY FIVE-SIX
Wasted a ton of time on making the top and bottom holders (out of carbon fiber too), and with 3D printed holders (very very unstable and inconsistent). Making them took a LOT of time because i was trying to make an equilateral triangle and trying to adjust the rods and the holders and everything, which took 2 days sadly

Corner holders:
![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/46a38859229804d12e5c2d0118798df3440be230_screenshot_20250628-085456.png)
these weren't practical or accurate at all, but this is what it looked like

## DAY SIX-SEVEN
Did some chatGPT-ing for design ideas, and also realised carbon fiber rods were insanely impractical and unstable, so i decided to make the frame out of 2020 AND 2040 extrusions. Also found something called "Kossel-style corners" which are 3D printed holders for the frame
![kossel corners](https://hc-cdn.hel1.your-objectstorage.com/s/v3/8a7604047e90eb4ef0b0df3963680a9203d99c77_img_0406.jpg)
![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/f475f5214940dc7380f694d27d2b6b7d532c8e06_img_0405.jpg)
![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/166e2051e640e8bdc4808fcce23239e446d3f43c_img_0404.jpg)

I also designed the carriage today:
![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/ef8303c50a4711215ca1f171c3fa7ccdd9aba0fc_img_0408.jpg)
![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/8a7604047e90eb4ef0b0df3963680a9203d99c77_img_0406.jpg)


## DAY EIGHT
EXTRUDER SHOPPING !! im using a bowden setup, and all hotends are either more expensive than my entire printer or slow and generic. My custom hotend assembly would be made of a V6 heatsink, 65W heat cartridge (not the best, ik, but it fits in my power budget of 100W for USBC), a volcano style heatblock, CHT 0.4mm nozzle, and a bimetal heatbreak.

Volcano heatblock (slightly different from V6, provides better heat retention (needed for low wattage heater):

![Screenshot 2025-06-28 at 4 14 47 PM](https://github.com/user-attachments/assets/d5832562-6553-4279-9ab4-93b98a9eafd1)

CHT nozzle with 3 holes for better melting efficiency:

![Screenshot 2025-06-28 at 4 18 40 PM](https://github.com/user-attachments/assets/7d97036f-7f84-475a-bb57-4e15fd1c525d)


## DAY NINE
Curated the BOM, currently, the printer costs about 100USD (1/3rd of the max budget). (remind me to keep making the BOM alongside the printer design process :sob:). Also, i've decided that for the printer, I won't be using a motherboard, but use an RPi Zero (which i have at home) giving it wireless capabilities, running Klipper. But a bit of research revealed that it's GPIO isn't fast enough, and thankfully I also had an orph Pico from highseas lying around, which is much more suitable for swiftly controlling motors.

## DAY TEN-THIRTEEN
Wasted a ton of time again, this time for designing the effector (the hotend carrier). I had to design a duct for the 5015 blower too, and made 3-4 iterations of it, but finally settled on a super simple duct and overall design, and also looks great.
I even found a set of 12 threaded balls and sockets (called 5347 rod ends), which was really helpful since the 3D printed ones wouldnt give a lot of freedom of movement.
![Screenshot 2025-06-28 at 4 20 42 PM](https://github.com/user-attachments/assets/507b3bdf-74cb-45fe-9db7-881fd83b56eb)

I also found out that these are for 3mm rods, so i had to design an adapter for my 6mm rods:
![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/e49f08b74417b5816ad6a0c806ddaac74bfa6177_img_0409.jpg)

## DAY FIFTEEN
I'll try to submit the printer finally today, so the documentation, logs, final BOM, including the most important parts-- USBC PD negotiation board and all the small parts needed to make it work, like buck converters, boosters, etc. finishing touches-- I'll get all that done today and submit it :D

This is a USB-C-PD Decoy board, which negotiates PD (upto 100W) with the power source.
![Screenshot 2025-06-28 at 4 46 29 PM](https://github.com/user-attachments/assets/6af279ec-269a-4f9d-82ea-cc379ece18f1)

## DAY SIXTEEN-SEVENTEEN
Worked on BOM, finishing touches here and there, and finally submitting it after 40+36 hours 😭

here are some images for you :)
![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/8a4dcad0904abcef704119de1344ff9c21bd588e_img-20250609-wa0000.jpg)
![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/85646aa2813d91d2908066b0b6b41089a6ea1d99_img-20250609-wa0001.jpg)
![](https://hc-cdn.hel1.your-objectstorage.com/s/v3/7a84de9ee1d1bf4c3e9fcd3e8fa14ff9d337cd1a_img-20250609-wa0002.jpg)
