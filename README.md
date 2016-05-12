# BeagleBox and Beagle Box 2

1. BeagleBox: [Build a dirt cheap, tough-as-nails field computer in a Pelican case](http://www.southernfriedscience.com/build-a-dirt-cheap-tough-as-nails-field-computer-in-a-pelican-case/)
2. BeagleBox2: [The BeagleBox 2: a dirt-cheap, tough-as-nails, 3D-printed, versatile field laptop.](http://www.southernfriedscience.com/the-beaglebox-2-a-dirt-cheap-tough-as-nails-3d-printed-versatile-field-laptop/)
3. BeageBox2: [Build your own BeagleBox 2!](http://www.southernfriedscience.com/build-your-own-beaglebox-2/)

###Background

Fieldwork is tough on equipment. You’re in the elements, facing wind, rain, and salt spray, sometimes on an open boat far out in the Atlantic. You and your gear takes a beating. But you’re out there because there’s science that need to get done, and often that means bringing a computer with you.

###Overview

Field equipment is often controlled via computer, and data entry mandates a computer, which means laptops need to be able to go out in the field. For graduate students and early career scientists on very tight funding budgets, this can be a dilemma. I’ve see the calculations happen as my colleagues prepare for the field: *do I take my one and only computer out into the field and risk damaging it, or do I leave it brute-force my way through sampling without it*. 

This equation is, counter-intuitively, getting worse. Sensors, sampling devices, and scanners are cheaper and lighter than ever before. Rather than buying a $20,000 piece of equipment, you can get a $20 plug-and-go component. The trade off is that these systems rely on external processing power, they need a general computer. That means your laptop is coming with you.

The BeagleBox and BeagleBox 2 are designed to solve this problem. Rather than taking your primary computer out into the field, the BeagleBox proves a basic, tough, expendable option that is cheap to build and even cheaper to replace. As single board computers like the BeagleBone, Raspberry Pi, and Pine64 become cheaper and even more powerful, the Beagle Box can be continuously upgraded. 

###Project Status

The first BeagleBox was a proof-of-concent prototype running Linux and LXDE on a BeagleBone Black. The case is basic and supports a 4-port USB hub and will fit most smaller, Raspberry Pi-size SBCs (single board computer).

The BeagleBox 2 has been totally redesigned with an easy to assemble case that is tougher and allows for greater functionality. It supports a 4-post USB hub, audio out, ethernet-out without going into the case, and an external power port. It runs Ubuntu on a Pine64 SCB. Both BeagleBoxes can handle 12V DC power, which allows users to hook up to a variety of power options. 

The BeagleBox 2 is field ready, and has been used to run an OpenROV and a Printrbot 3D printer, as well as perform standard computational tasks. 

###Bill of Materials

Almost all of the necessary parts can be found through Amazon. Visit our [Parts Depot](http://oceanographyforeveryone.com/depot.html) for the full list. Pine64 boards are available from [Pine64.com](https://shop.pine64.com/).

###Build Instructions (for both BeagleBox and BeagleBox 2 unless noted)

1. Confirm the screen and single board computer work by connecting through the HDMI and powering up both devices independently. Be careful not to connect the 5V SBC to a 12V power adapter. 

2. Solder the input side of the 12V to 5V converter to the 12V and ground outputs on the JB Tek/Tontek/Screen control board. Solder a 5.5mm barrel plug to the output side of the converted (for SBCs that use microUSB power, attach an adapter to the barrel plug, or directly hard wire a microUSB plu to the converter output, though this ill limit your options for swapping SCBs later). You can now power both the screen, which needs 12V, and the SBC, which needs 5V, off a single AC adapter. Because 12V direct current is relatively ubiquitous, you can run the computer off a boat battery, car battery, or any of dozens of different battery options without any special converters. Just make sure the amperage isn't much above 2000 mAh. 

3. Connect the HDMI input, USB hub, wifi adapter (optional), and audio adapter (optional), as well as your USB keyboard and mouse of choice. **BeagleBox 2:** Connect a male barrel plug to the female barrel jack and connect to 12V power on the screen control board. Power on and ensure that all components are functioning properly. 

4. Print the case. **BeagleBox:**Arrange all of the screen pieces and ensure that you have them in the correct orientation. Using hot glue, affix all the screen components together using the individual tabs for added support. Attache the screen to the back of the frame using heavy-duty tape. The two case components can be held in with friction, but a few dabs of hot glue will lock them in place. **BeagleBox 2:** The screen is designed such that it can only be assembled one way, dramatically simplifying the build. Use hot glue on the edges and overhangs to assemble the screen frame, then affix the screen with heavy-duty tape. The assembly fits *very* tightly into the Pelican case, but a few extra dabs of hot glue on the edges will prevent things from moving around. The case coms in four parts, which can be hot glued together along the edges and overhangs. Start with the lower parts and then affix the upper two quarters after all connector have been passed through. Glue the connectors into place with a dab of hot glue. 

5. Tidu up the case. I use velcro tabs to keep everything from moving around inside the case and try to scrape as much excess hotglue off as possible to keep everything looking neat.  

6. Download your prefered distribution of Linux and flash to your SCB. 

###About the Beagle

I named the first BeagleBox after the BeagleBone Black used to power it. Since the BeagleBox 2 no longer uses it, I'm going to declare that all future iterations of the BeagleBox are named for the *HMS Beagle*, in honor of one of the greatest field biologists of all time.

###Acknowledgments

The BeagleBox and BeagleBox 2 were designed by Andrew Thaler. 

###Code of Conduct

Please review our [Contributor Code of Conduct](https://github.com/OceanographyforEveryone/BeagleBox/blob/master/CODE_OF_CONDUCT.md) prior to your first contribution. 
