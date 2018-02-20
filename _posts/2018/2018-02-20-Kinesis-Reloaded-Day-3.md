---
layout: page
title: "Kinesis Reloaded: Day 3"
subheadline: "Modification Log - Kinesis Contoured Model 110"
teaser: "In the final part of this series, all the pre-assembly work has been completed. All the various parts of the Kinesis have been overhauled and modernized. The last step is to assemble it!"
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

Previously: [Kinesis Reloaded: Day 2]({{ site.baseurl }}/keyboards/2018-02-13-Kinesis-Reloaded-Day-2)

<div class="video-responsive">
    <iframe width="640" height="360" src="http://www.youtube.com/embed/ycS9kv-ioRA" frameborder="0" allowfullscreen></iframe>
</div>

Once again welcome back, loyal readers. This will be the final post in the Kinesis Reloaded series. After ages of dreaming of a Kinesis of my own, and year of acquiring parts - the Kinesis Contoured is finally complete!

Above is the video build log for this board. In it I go through the build from start-to-finish.

All the work on this board was performed in marathon build and mod sessions - 3 different days across 3 weeks. The last session was prep for the RGBs and final assembly.

In previous posts, I detailed the prep work that happened before this final assembly:

+ Desoldered all switches and diodes on the Kinesis Contoured
+ Desoldered all switches and diodes on the Kinesis Advantage donor board
+ Installed Otemu Ice switches + Advantage PCBs on the Contoured keywells.
+ Assembled and flashed the Stapelberg controller PCB
+ Tested and verified RGB was working in the firmware.

#### Day 3

With all the prep work for the Kinesis' various parts in order, the last steps before assembly were to install some sound dampening and wire up the RGB strips.

##### Resonance

<center>
<a href="https://imgur.com/jDmrdNx.jpg" data-fancybox>
	<img src="https://imgur.com/jDmrdNx.jpg" alt="" />
</a></center>

I noticed early on that typing on the Kinesis boards (both the Contoured and Advantage) yielded a very 'pingy' experience. Specifically because of the case's somewhat resonant design, typing causes the switches' springs to resonate and 'ping'. To
alleviate this, I installed some level of sound dampening.

I've got a ton of old mousepads hanging around the house, so I went through for the top and bottom parts of the case and cut out mousepads and adhered them to the case. The mousepads aren't able to completely fill the space inside the case, so there is still some ping left, but it's largely been reduced in the final assembled board.

##### RGB

<center>
<a href="https://imgur.com/enAe1Oi.jpg" data-fancybox>
	<img src="https://imgur.com/enAe1Oi.jpg" alt="" />
</a></center>

In previous testing on the board, I verified that the firmware was working, and that I'd properly wired a test RGB strip. The task before assembly was to wire up 6 separate strips and get them going.

In previous builds I've used RGBs, and have even ran them in parallel before (like my ErgoDox test board). With the Kinesis I used more RGBs than I've ever used before. 6 strips, with a total of 40 LEDs.

Prep for this went well. I wired up the 6 strips, running leads from each for 5V, GND, and Data. I was genuinely surprised when they all worked the first time I fired the strip up. Once I knew the strips were working, I placed and adhered them down in the case.


#### Assembled

<center>
<a href="https://imgur.com/iyWSh9k.jpg" data-fancybox>
	<img src="https://imgur.com/iyWSh9k.jpg" alt="" />
</a></center>

With all the parts ready, I installed them and got the board assembled.

I'd expected that after assembly I might need to do a bit of tweaking with the RGBs, but I was pleasantly surprised by how well the light shines through the switches. There are a **lot** of LEDs in this case, but I still didn't expect this much light.

Now completed, the board looks great, and feels amazing to type on. Outwardly, with its factory case and keycaps, the Kinesis Contoured would appear to be completely unmodified (as long as the LEDs are off of course). I achieved the 'sleeper' look that I was shooting for. This board looks **exactly** as I wanted it to.

Typing on the Contoured feels fantastic. I'm a big fan of tactile mechanical switches, and these Otemu Ice switches (75g) do not disappoint. They're a significant improvement over the Cherry Browns that were in this board previously - heavier, smoother, more tactile.

<center><ul class="clearing-thumbs small-block-grid-4" data-clearing>
  <li><a href="https://imgur.com/q9jLlU4.jpg"><img data-caption="" src="https://imgur.com/q9jLlU4.jpg"></a></li>
  <li><a href="https://imgur.com/5miuvE0.jpg"><img data-caption="" src="https://imgur.com/5miuvE0.jpg"></a></li>
  <li><a href="https://imgur.com/ui9DsfS.jpg"><img data-caption="" src="https://imgur.com/ui9DsfS.jpg"></a></li>    
</ul></center>

Naturally, this entire process could have been simpler if I'd just installed new switches in my Advantage donor board and called it done. That said, I'm rarely one to take the easy and simple way on personal projects. After I bought the Contoured a year ago in nonworking condition, I really fell in love with the white case and keycaps. Most Kinesis boards are just a simple black, so I loved the look of the white - it was important that any finished Kinsis board I have use the white case. Without all this work, I simply couldn't have a board that looks and works like this.

It was also important to me that I have programmability. The default layout on Kinesis boards is excellent - probably the best keymap and built-in function layers that I've seen on a production keyboard. Despite how great these boards are from the factory, it's important to me that I be able to customize a keyboard's layout (and function layers) to best fit how I like to use a keyboard.

For those that are interested in seeing my keymap, or how RGB was set up on this board - my keymap is [here](https://github.com/missourivalleytech/qmk_firmware/blob/master/keyboards/kinesis/keymaps/cheddarbek/keymap.c), and my copy of the firmware is on Github [here](https://github.com/missourivalleytech/qmk_firmware/tree/master/keyboards/kinesis).

This build has been a long time coming, and I'm so glad to see it finished, and to reap the rewards.

---
<p align="right">Typed on Kinesis Contoured</p>
