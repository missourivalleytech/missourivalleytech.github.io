---
layout: page
title: "Kinesis Reloaded: Day 1"
subheadline: "Modification Log - Kinesis Contoured Model 110"
teaser: "After a year of making small plans and acquiring parts (namely a Stapleberg controller), I was ready to start modifications to the Kinesis. Last Sunday was Day 1 of a multi-part project. These modifications will completely rebuild the Kinesis from the ground up. When I'm done, the only thing that will remain from the original board is the case."
author: Morgan
categories:
  - keyboards
image:
    title:
    homepage:
    thumb:
    caption:
    caption_url:
breadcrumb: true
comments: true
---

Previously: [Kinesis Reloaded: Day 1]({{ site.baseurl }}/keyboards/2018-01-30-Kinesis-Reloaded-Day-1)

Welcome back, loyal readers. In the previous part of this adventure in Kinesis modifications, I had completed all the preliminary prep work on the Kinesis' left and right keywells, and thumb clusters. The keywells and thumb clusters had new Otemu Ice switches soldered in, and I had verified (using the stock control electronics) that the PCBs and thumb clusters were working as expected.

This past Sunday I spent my day working on the Stapelberg Controller, validating that I could upload a firmware to the controller, sorting out the pin configuration for the thumb clusters, and adding RGB lighting to the board.

As stated in previous posts, this project is a total overhaul of my Kinesis Contoured Model 110. From it, the case will be the only original part left.

##### Project Goals

+ Replace factory Cherry MX Brown switches with tactile Otemu Ice switches. - **DONE**
+ Replace period keywell and thumb cluster PCBs with modern (Stapleberg compatible) PCBs. **DONE**
+ Replace factory control electronics with Stapleberg controller. **DONE**
+ Add RGB underglow. **DONE**

There is also a _new_ project goal that I will explain in more depth later in this post.

+ Get Fkey row of non-mechanical switches working with the Stapelberg controller.

#### Day 2

Day 2 was largely test and validation day. With all the hard work on the keywells and thumb clusters complete, I knew that the majority of the work remaining would be testing and troubleshooting issues with the build.

##### Stapelberg

<center>
<a href="https://imgur.com/KqmHOVh.jpg" data-fancybox>
	<img src="https://imgur.com/KqmHOVh.jpg" alt="" />
</a></center>

The first order of business was to prep the Stapelberg Controller itself. For this, headers must be soldered to the circuit board, followed by the Teensy controller. The standard build instructions for this are to use white vertical-insertion headers for the keywells and Fkey rows, and to solder thumb cluster wires direct to the controller. I opted for a couple changes to fit this board.

1 - Instead of wiring the thumb clusters direct to the controller, I instead opted to wire sockets to the controller, and headers to the thumb clusters. This allows me to then use jumper wires to connect the two. In hindsight this wasn't really needed, since the thumb cluster wire arrangement is pretty straightforward, but I made the choice so that if I had to do some tweaking all I would need to do is move jumper wires - rather than resolder.

2 - Instead of using the white vertical-insertion ribbon headers for the FKey row, I again opted for sockets. I chose this because I wanted to use the original Kinesis Contoured's white Fkeys and circuit board. This older Contoured Fkey circuit board uses header pins instead of a ribbon. By using sockets on the Fkeys pins on the Stapleberg controller, I'd give myself room to play with the wire arrangement. I figured that it was likely the wiring was different between the Contoured Fkeys and the Advantage FKeys that the Stapelberg controller was designed for.

With all the headers and sockets on the controller, next I added the Teensy. Unlike most keyboards that use a Teensy - this one has the teensy face-down. With this arrangement, it's not possible to access the Teensy's hardware reset button - something to be mindful of if you undertake a mod like this. Given that I wouldn't have access to the reset button, I opted to add some headers to the GND and RST pins on the teensy - that way I could jump those two pins to reset it when need be.

I also added headers to the A port pins on the teensy, so that I could use one of them for data to my RGB strip. And also to the 5V pin, for power to the RGB strip.

##### Flashing & Testing

With all the prep work done on the Stapelberg controller, it was time to flash a firmware and get to testing things.

Oh boy, this part took me forever. It was a big change for me to adjust to when the ```make``` commands got changed in QMK back in October. With those changes, I always feel a lack of confidence anytime I try to flash a new QMK board. I won't lie, I spent a good hour or two fighting with QMK trying to get a firmware flashed.

With this particular keyboard in QMK, there are two projects under the /Kinesis directory: /avicstep, and /stapelberg. Anytime I tried to even _compile_ the Stapelberg firmware I got a rules error. As it turns out, I'm a moron that was typing stap**le**berg, rather than the correct stap**el**berg.

Once the controller was flashed, I was able to test and verify that the keywells and thumb clusters were working with the new controller.

##### RGB

Next up was RGB. In the past RGB was always something I found too intimidating to add to a board of my own. Anytime I used RGB it was limited to boards where someone else had already added the RGB functionality to the firmware (like DZ60 or Iris). In the past couple years though QMK has made the process for adding RGB much **much** easier.

First I took care of the hardware side - I soldered three jumper wires (for 5V, ground, and data) to an RGB strip. Then I connected jumper wires to 5V, GND, and A3 pins on the teensy. The A3 pin serves to transmit data to the RGB strip.

<center>
<a href="https://imgur.com/fiXOYvP.jpg" data-fancybox>
	<img src="https://imgur.com/fiXOYvP.jpg" alt="" />
</a></center>

Adding RGB functionality to the firmware was a BREEZE. Far easier than I thought it would be. As it turns out, all the RGB functionality is now in QMK by default, and for the firmware it's just a matter of adding the right lines to the keyboard's project files.

Inside the _config.h_ file at ~/Kinesis/Stapelberg/config.h I added these lines:

```
/* ws2812 RGB LED */
#define RGB_DI_PIN A3
#define RGBLED_NUM 40
#define RGBLIGHT_ANIMATIONS```

In my keymap's _rules.mk_ file at ~/Kinesis/keymaps/default/rules.mk I added:

```RGBLIGHT_ENABLE = yes
```

With that, RGB was enabled and functioning in my firmware. The last step was to add actual keycodes to my keymap to control the RGB. In my keymap I have a keycode for ```RGB_TOG```to allow the strip to be turned on and off.

<center>
<a href="https://imgur.com/ONU9wmw.jpg" data-fancybox>
	<img src="https://imgur.com/ONU9wmw.jpg" alt="" />
</a></center>

I then flashed the Stapelberg controller and validated RGB was working. Awesome!

##### Fkeys

As stated above, one of the last goals before I got to final assembly of the Kinesis was getting the non-mechanical Fkey row working with the Stapelberg. When I was prepping the Stapelberg I added sockets so that I could use jumpers from my original Kinesis Contoured Fkeys to the controller. As it turns out, this was a mistake.

I had anticipated that the Contoured fkey circuit boards would have a different layout than the Advantage fkeys, but I had no idea how different it would be. In short, the Controured's fkeys use a wiring matrix like I've never seen in a keyboard before.

<center>
<a href="https://imgur.com/JbCUWpk.jpg" data-fancybox>
	<img src="https://imgur.com/JbCUWpk.jpg" alt="" />
</a></center>

Before I started trying to make the fkeys work, I had assumed (incorrectly) that it would be a 1:1 pin mapping. 9 keys, 10 pins - I figured one pin for each button and another to complete the circuit. Boy howdy was I wrong. Though the Fkeys are just one row, the wiring goes all over the place. Esc is wired to F1 and F2, F2 is also wired to F5 and F6, F6 is also wired to F3 and F4, it's just a mess.

<center>
<a href="https://imgur.com/FKCHqxy.jpg" data-fancybox>
	<img src="https://imgur.com/FKCHqxy.jpg" alt="" />
</a></center>

I tried and tried for a couple hours to find the right combination and arrangement of pins from the Fkeys to the Stapelberg, but I never could sort it out.

After a wasted couple hours trying to make them work, I feel back on my parts board and harvested the fkey ribbon cables from my Advantage donor board, installed the correct ribbon headers in the Stapelberg. It took a bit of finessing to get the ribbon cables situtated in the case, behind the rubber buttons, but eventually I got it all installed.

While I did fail at getting the original Controured Fkey PCBs to work, I did at least reuse the original rubber buttons themselves, so the Fkey row appears to be factory an unmodified from the outside.

#### Ready To Assemble

With the Fkey rows sorted out, all parts of the build were validated and I knew they were working properly. Most of the testing thus far had actually taken place with raw components outside of the case - I had wiring everywhere and the case was a mess. The day was getting late, but I knew it was ready for the last part - assembly, which I'll save for the last part of this series.

Stay tuned!

---
<p align="right">Typed on Blue Alps64</p>
