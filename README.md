# BeagleBox

[Link](http://www.southernfriedscience.com/?p=18661): Southern Fried Science Project Desription

###Background

Fieldwork is tough. You’re in the elements, facing wind, rain, and salt spray, sometime on an open boat far out in the Atlantic. You and your gear takes a beating. But you’re out there because there’s science that need to get done.

###Overview

Field equipment is often controlled via computer, and data entry mandates a computer, which means laptops need to be able to go out in the field. For graduate students and early career scientists, this can be a dilemma. I’ve see the calculations happen as my colleagues prepare for the field: *do I take my one and only computer out into the field and risk damaging it, or do I leave it brute-force my way through sampling without it*. That is, if they’re lucky enough to have alternative methods they can employ. For some gear, there’s no choice but to take the computer.

This equation is, counter-intuitively, getting worse. Our sensors, sampling devices, and scanners are getting cheaper and lighter. Rather than buying a $20,000 piece of equipment, you can get a $20 chip, but there’s a trade off, and the trade off is that chip based systems rely on external processing power, they need a general computer, and that means your laptop is coming with you.

I don’t like going out on the water with my laptop. Losing it would be frustrating and time consuming. It’s tough, but it’s not tough-as-nails. And it’s definitely not cheap.

So I tapped into the wealth of Maker experience I’ve accumulated over the last few years and build a new one, using a single board computer, some extra peripherals, and a 3D printer. And I shoved the whole thing into a Pelican case. Say hello to the BeagleBox, a dirt cheap, tough-as-nails field computer for about $200.

###Project Status

We have a single proof-of-concent prototype running Linux and LXDE on a BeagleBone Black. The case need to be updated to be more useful in the field, we need to add a battery system for more portability, and I'd like to swap out the BeagleBone for a RasberryPi++. 

###Bill of Materials

Almost all of the necessary parts can be found through Amazon. Visit our [Parts Depot](http://oceanographyforeveryone.com/depot.html) for the full list.

###Build Instructions

Building a BeagleBox is pretty simple. The heart of the machine is a BeagleBone Black, a small single board computer. You are definitely not going to be blown away by its 1 GHz processor, but we’re not building a high-throughput genome analyzer, here, we're building something that can handle the basics and get beat to hell. 

All told, the BeagleBox tops the scales at a touch over $212, and that’s if you bought everything new. To connect all the electronics, I first soldered the 12V to 5V converter directly to the 12V and ground outputs on the JB Tek control board, then pulled the barrel plug of the 5V AC adapter and wired it into the converter’s output. The result is that you can now power both the screen, which needs 12V, and the BeagleBone, which needs 5V, off a single AC adapter. As an extra bonus, the BeagleBox now needs 12V direct current, so you can run the computer off a boat battery, car battery, or any of a squillion different battery options without any special converters, all you need is a the right plug or clamps. (and, of course, watch those amps).

The BeagleBone sends video out a micro-HDMI port, the monitor accepts standard HDMI, so you need a the right cable to connect the two. After that, all you need is to plug a USB hub into the single USB port, and you’re ready get your software set up.

I use the latest Debian image from BeagleBoard.org (did I mention this is a Linux machine?) paired with the LXDE light-weight GUI. If you’re new to Linux, now is a good time to read up on the basics of the operating system and familiarize yourself with how it functions, but once you have LXDE installed, you’ll have a reasonably intuitive desktop with a start bar and some basic programs. You’re going to want a mouse and keyboard, any USB devices will do, but I like this one, for its simplicity. If, however, you’re mostly going to use this for something other than data entry (for example, flying an OpenROV), one of these little guys will actually fit in the Pelican case with everything else.

Now, for the fun part, 3D printing. I designed a shell around a Pelican 1200 case. It’s just the right size for the screen and gives you plenty of extra space to store whatever else you need to store in the case. The shape files are available on YouMagine. I printed everything on a PrintrBot Simple Metal, with no problem.

To assemble the shell, I use SciGrip4 Acrylic solvent and hot glue, but any adhesive will do. Hot glue seems to take to PLA particularly well. The small tab brackets go on the back of the screen mount, and both hold the frame together and keep the screen in place. The main shells slot into the Pelican case and are help on with a little bit of hot glue. The USB hub slides through the large rectangular port and the power cord comes out the small semi-circle. Everything should be very snug.

And with that, the basics are done and you have a bare-bones field computer. Not only that, but by the end of this build, you should have the confidence to expand on this design. There’s a million different ways to modify it to suite your needs.

###Resources

[Oceanography for Everyone](http://oceanographyforeveryone.com/)

[Original Project Description](http://www.southernfriedscience.com/?p=18661)

###Acknowledgments

BeagleBox was designed by Andrew Thaler. 

###Code of Conduct

Please review our [Contributor Code of Conduct](https://github.com/OceanographyforEveryone/BeagleBox/blob/master/CODE_OF_CONDUCT.md) prior to your first contribution. 
 
