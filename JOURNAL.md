Made by: @aryan
Repository link: https://github.com/aryn-pathak/material-zero/
Total hours so far: 39.5 Hours (wished i worked 30 mins more to hit 40 :heavysob:)

Massive thanks to Hack Club and Alex for giving me this insane opportunity to build my own 3D printer!

This is Material ZERO (zero for being the zero-th version of a printer that will be heavily modified to make better versions down the line.), A printer that is easy to modify, upgrade, and most importantly-- to use.
- Features a truly hands free experience for printing; simply uploading an stl file on the web interface and choosing a preset (fast, hi-res, fast with supports, or hi-res with supports). That's it: slicing, supports, settings, ABL, all handled by Material.
- The printer also features a magnetic printhead (with wiring!), so swapping out toolheads is just a click of neodyium magnets away!

- [x] I have access to a 3D printer (printing-leigon)

BOM: https://docs.google.com/spreadsheets/d/1OtqszPI16ybW3s_6Pz4gcUsUTPw2b_rEn2WlHAjkEtA/

## DAY ONE // 18th March
- I'm new to this so I did a ton of research today :D. I have gained an understanding of mechanisms, and feel much more confident now!
- Research time: 1 hour

## DAY TWO // 19th March
- Curated the BOM today, and I have a vision of what I want my printer to have:
- ~~Should have USBC, Portable, size perhaps 55 x 55 x 55, Battery powered (obvio). Preferably but not compulsorily wireless~~
- ~~Since this is going to be portable, the hotbed should have a firmer grip.~~ I would've loved these features but it'd be hella impractical and slow and inefficient 
Time spent: approximately. 30 mins

## DAY THREE // 21st March
- I need to lock in for the next ten days now.
- Im making the BOM in google docs now, and the parts I found out earlier are now out of stock/very low stock, so I'll make a BOM from novo3d.in
- Also, I have decided to make a slightly different kind of printer, new requirements:
    - ~~USBC~~, WiFi/BLE compatibility
    - Should be fast
    - It should continue printing right where it left off in case of power outage
    - Should have a camera and software to create good timelapses
    - It will also have a grid of neopixels to indicate the progress
    - It will have a touch display which can show contols, progress (in time) and estimated time remaining.
    - The camera should be able to stream the progess if requested by user wirelessly.
 
- Time spent: 30 mins

## DAY FOUR // 22nd March
- Got a lot of progress on the BOM, now I can start working on CAD
- I need to watch a tutorial on FreeCAD
- I also got another insane idea: what if the printer could make filament out of random plastic pieces? (note from future: will add this feature through a custom printhead/bottle cutter filament thing that I'll print with my printer)
- Time spent: 2.5 hours

## DAY FIVE // 23rd March 
- Yesterday night, while racking my brain, I decided to make a bedslinger instead of X and Y axes being controlled by the printhead.
- X and Z axes will be controlled by the printhead, Y will be controlled by the heatbed. 
- X and Y to be controlled with belt and Z will be controlled by lead screws.
- Another idea: I have found a yt video to directly print plastic shreds instead of making filament first. For this, the printhead has an extension on top of it (like a hat).
- However this modified printhead will not be able to print filament. To solve this problem, I will have two printheads, which can be swapped magnetically.
- The bracket which is controlled by the belt will have neodymium magnets embedded. the swappable printheads too will have magnets embedded.

- I found this resource: https://www.instructables.com/DIY-3D-Printer-From-Scratch/ which has helped me a TON! Everything just got a who lot easier, because I had so many misconceptions regarding the structure and mechanisms.
- I will be ditching the linear rails entirely and use smooth rods.
- Also, my old bracket for the belt was supposed to be attached to the belt using grooves, but watching a video, I can just attach it using a ziptie.
- Also, I will now be using open belts instead of closed ones, which is a good thing, because I couldn't find an appropriate size for the belt.

- Finally got started on CAD today, (only started tho 😬)
- Need to get much much more productive tommorow 

Time spent today: 2 hours (was planning on 5 tho)

DAY SIX // 24th March
- I was quite productive today, much progress on CAD (completed X and Z axes):

![X and Z axes](https://hc-cdn.hel1.your-objectstorage.com/s/v3/51154a908ddcd4e170b69a1fa0464eb5b0e29f78_img_0326.jpg)

- I'm hoping I can complete the Y axis aswell, and then complete the printhead and heatbed tommorow, but I have homework to do :heavysob:

- Sadly I wasn't able to continue any work after this, but I will make some sketches tonight for the Y axis, and maybe of the structure too.

- I'm also thinking of making my own motherboard, as it gives me full freedom, however, I'll have to research before I can commit to it. (I also wanted to make my own firmware but I figured time isn't on my side and it's overkill)

- Also, here are some of my sketches of old and new designs so far:
![sketch1](https://hc-cdn.hel1.your-objectstorage.com/s/v3/6f355e900b0061c73665333bd9642c0225e2e9a8_img_20250324_225829691_2.jpg)
![sketch2](https://hc-cdn.hel1.your-objectstorage.com/s/v3/4234bece10737d80410451c42806a35a03824194_img_20250324_225758611.jpg)
![sketch3](https://hc-cdn.hel1.your-objectstorage.com/s/v3/a2265cf7e93b79f979d287e90ee0cce002096f21_img_20250324_225712216_2.jpg)

I love how messy they look :D

CAD: 3 hours

DAY SEVEN // 25th March
- I got straight into PCB design for the motherboard, but I'm reconsidering now, maybe I don't need to make my own motherboard.
- If I'm done with the entire thing and still have time left, I'll start working on it.
- Also, some research revealed I can't use USBC to power the printer D:
- Quite some progress today, worked on Y axis (all 3 axes successfully done)
- I can get to making the printhead and structure tommorow.
- If I have time, I'll make my own motherboard with an rpi zero W as the controller (I have some)

Here's the CAD till now:
![CAD](https://hc-cdn.hel1.your-objectstorage.com/s/v3/916e223f7d019f3a60dcb6d4e93ef999c94f1ff4_img_0328.jpg)

![CAD2](https://hc-cdn.hel1.your-objectstorage.com/s/v3/525c021bc8332c72f5caf2e0854ef1367404aa72_img_0330.jpg)

Research: 2 hours, CAD: 2 hours.

DAY EIGHT // 26 March
(logging on 27th March)

- Couldn't get much work done today, but did some research and found a nice midrange motherboard and found a great extruder kit (Titan kit) for quite cheap!
![titan extruder kit](https://hc-cdn.hel1.your-objectstorage.com/s/v3/81b9cd3318ebc249dc070a838d3868e34c5ba1fb_img_0332.jpg)
![titan extruder kit](https://hc-cdn.hel1.your-objectstorage.com/s/v3/48ccb7ab9130cc862169591c919dbcd0a6203735_img_0331.jpg)
research: ~45 minutes

DAY NINE // 27 March

- Finished frame today :D (fixed a lot of errors in the model too)
- Researched a bit too
- Had some progress today, but not nearly as much as I had planned :heavysob:

research: 45 minutes 
CAD: 2 hours

DAY TEN // 28 March

- Refined the frame today, built the magnetic toolhead and the adapter for my titan extruder!!
![toolhead](https://hc-cdn.hel1.your-objectstorage.com/s/v3/b3690f2c58986f4b36e526681b818ef2d066cf56_img_0335.jpg)
![toolhead](https://hc-cdn.hel1.your-objectstorage.com/s/v3/bcf26836a9ae620402b81ec7d6a0e919937cf2bb_img_0334.jpg)
![toolhead](https://hc-cdn.hel1.your-objectstorage.com/s/v3/fb90b902f9c20059bca4af246f1f7d97c6171a42_img_0333.jpg)
- Completely finished with my printer... or so i thought 
![printer](https://hc-cdn.hel1.your-objectstorage.com/s/v3/a559a3c203438644a7c983c075a69d37a633c0ba_img_0336.jpg)
- I talked to some people on slack and research a bit (a lot), and I'm gonna use extrusions for the frame.
- Luckily I found some mounts on novo3d which fit perfectly with the 2040 profile extrusions.
- I started working on the new frame, but I'll do the rest tommorow.

Research: 2.5 hours (approx)
CAD: 2.5 hours

DAY ELEVEN // 29 March
- Made progress on the Y axis using extrusions, but I need to figure out how to connect the belt to my heatbed. Gonna use Gantry beds instead of rods for the Y axis.
- Also made a bracket to connect the Z axis to the extrusions.
- Much less progress than I hoped for, but I'll finish the printer by tommorow most likely.

CAD + some research: 2 hours 25 minutes

DAY TWELVE // 30 March 
- Completed the printer with extrusions today :D
- I'll use the remaining days to work on finishing touches and adding features.
- Didn't get research done today since I was traveling tho

![printer](https://hc-cdn.hel1.your-objectstorage.com/s/v3/1bd5ba2f538b27c5319706f278c6a651c9f859e8_img_0342.jpg)

CAD: 3 hours 

DAY THIRTEEN // 31 March
- Today is mostly for research and implementing special features.
- For now, scratch the vision for my printer I had mentioned before, for now, the printer will have the following features:
    - Hands free printing: I want to build a printer that requires minimal human input and contact with the printer. I will connect a raspberry pi zero to the motherboard to add more features and use a web interface for starting prints automatically.
    - I also don't want to spend too much time fiddling with the print settings everytime I need to print something. I want to just plug it in, upload a file (remotely), and boom- all the settings will be configured by algorithms on the raspberry pi and the print will start.

DAY FOURTEEN // 6 April
- Worked on software only today
- The printer will be equipped with software for truly hands-free operation, which means the user just has to upload the STL file, which gets stored, sliced, with supports (if required).
- This will mean that a raspberry Pi will be connected to the btt e3 mini acting as the computer uploading the file. The firmware is in a very early age, and will get a lot of features later on yay

Code: 1 hour

DAY FIFTEEN // 7 April
- Pure CAD today. Absolutely nothing else.
- The deadline's closing in, and luckily because of my time zone (IST), this ends on 9:30AM on 8th april, so I'll make the PCB and code and the last bits of CAD early tommorow 🤞

CAD: 4 hours

DAY SIXTEEN // 8 April
- DONEDONEDONEDONEDONEDONE
- (woke up at 5:30, skipped school, finished the printer by 10AM)
- Finished CAD, Finished software, Compiled BOM (along with screws!)

CAD: 1.5h
Research, BOM, etc: 2h
Coding: 45 mins
(screentime shows music: 1h 45mins...?)
total: 4.5 hours
