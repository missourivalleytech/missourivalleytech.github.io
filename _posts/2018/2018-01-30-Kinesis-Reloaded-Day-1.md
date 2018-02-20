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
Previously: [The Stapleberg Controller]({{ site.baseurl }}/keyboards/2018-01-05-The-Stapleberg-Controller)

<center>
<a href="https://imgur.com/etkYCa3.jpg" data-fancybox>
	<img src="https://imgur.com/etkYCa3.jpg" alt="" />
</a></center>

It was roughly a year ago that I acquired a ~1995 [Kinesis Contoured Model 110 keyboard]({{ site.baseurl }}/keyboards/2017-02-09-Kinesis-Countoured-Model-110). Like many people, my first time seeing a Kinesis was in [Men and Black](https://www.reddit.com/r/MechanicalKeyboards/comments/27vkcg/keyboard_spotting_i_was_just_watching_men_in/). With its crazy design and sculpted keywells, I was really interested in this keyboard even then, long before I turned into a keyboard wonk. When I got this white Kinesis Contoured a year ago it wasn't fully functional, but I was happy just to have it. Even if I never did anything with it, the Kinesis is a fun board to put on the wall.

After a year of making small plans and acquiring parts (namely a [Stapleberg controller]({{ site.baseurl }}/keyboards/2018-01-05-The-Stapleberg-Controller)), I was ready to start modifications to the Kinesis. Last Sunday was Day 1 of a multi-part project. These modifications will completely rebuild the Kinesis from the ground up. When I'm done, the only thing that will remain from the original board is the case.

##### Project Goals

+ Replace factory Cherry MX Brown switches with tactile Otemu Ice switches.
+ Replace period keywell and thumb cluster PCBs with modern (Stapleberg compatible) PCBs.
+ Replace factory control electronics with Stapleberg controller.
+ Add RGB underglow.

#### Day 1

On Sunday I was at my workbench for nearly 8 hours - I only completed my two goals. Of course, desoldering two complete boards, then soldering in ~80 some switches does take quite a bit of time. Now that I'm halfway done, I'm hoping the remaining half can _also_ be done in a day.

The first order of business on Sunday was extracting the modern PCBs from a Kinesis Advantage. My white Kinesis Contoured is old enough that its internal design and circuitry is entirely different from the modern-day Advantage boards. As a result of these differences, the programmable Stapleberg controller is not compatible with the Contoured's circuitry. I could've alleviated myself all the headache of desoldering by just buying raw PCBs directly from Kinesis, but in the end the cost difference between raw parts and a used Kinesis Advantage was negligible. The route I chose was a lot more work, but I have the benefit of an entire spare Kinesis case for future projects.

<center>
<a href="https://imgur.com/BvOCehU.jpg" data-fancybox>
	<img src="https://imgur.com/BvOCehU.jpg" alt="" />
</a></center>    

To extract the PCBs, I first disassembled the Kinesis, whipped out my trusty [desoldering iron](http://amzn.to/2BEEmbC), then got to the business of desoldering the switches. I've desoldered quite a few keyboards in my time, but this was definitely the most difficult yet. For one, the Kinesis' matrix diodes are _inside_ the switches - so there's double the desoldering work to do just to remove a switch; secondly, the curved keywells make it very difficult to actually desolder the pins without damaging anything. It took me quite a long time just to get the solder out, then the same amount of time to actually get the keywell PCBs off without totally wrecking them. Despite all my caution, I did still damage the PCBs in several places, so patch wires were needed when I got to reassembly. I can't say that I'm too desperately surprised that the PCBs took some damage - unlike any other keyboard PCBs, these are flexible, so quite a bit thinner than anything else out there.

After removing the switches from the Advantage's keywells, I repeated the same process on the white Contoured's keywells. With the contoured I threw caution to the wind, knowing that I wouldn't be able to reuse the PCBs. Without care about the PCBs (since they'd be trashed anyway) the desoldering was much faster and smoother.

With the white Contoured's keywell bare, I installed the 75g Otemu Ice switches that I'll be using in this build. Otemu has come a long way in the past few years. Just 3 years ago every Otemu switch I tried was absolutely terrible; these new Ice switches are very nice, and make a great budget alternative to Zealios. The Ice switches are pretty smooth, and very tactile. Not as good as Zealios, but still pretty good (considering they're half the price).

<center>
<a href="https://imgur.com/MWypm7A.jpg" data-fancybox>
	<img src="https://imgur.com/MWypm7A.jpg" alt="" />
</a></center>

Next, were diodes. I've got a lot of experience working with diodes, many previous builds (Alps64, ErgoDox, Iris) have used them. Typically with diodes there is a dedicated through-hole space for them _next to_ the switch, with the Kinesis PCBs, the diode holes are _right under_ the switch. I decided that unlike Kinesis, I wouldn't put diodes inside my switches; if I ever wanted to change the switch type the desoldering work would be hell. I opted instead to put the diodes on the opposite side of the PCB and have them poke through. It took a bit to verify that my diode orientation was correct, but soldering them in was mostly painless. I did need to cut the soldered legs on the switch side of the PCB down totally flush, so the switches wouldn't be interfered with by the diode legs poking out from the PCB.

<center>
<a href="https://i.imgur.com/9aP2Bp1.jpg" data-fancybox>
	<img src="https://i.imgur.com/9aP2Bp1.jpg" alt="" />
</a></center>

With diodes soldered and the PCBs prepped, I started the task of soldering the PCB on to the switches. Funny...typically I think of soldering switches to the PCB, but for this build it's quite the opposite. The switches are first installed in the keywell plate, then the PCB is bent over the switches and soldered into place. This soldering work is complicated and time consuming, but after some creative work (holding the flexible PCB down as I soldered) I was able to get it done.

<center>
<a href="https://i.imgur.com/SGtZS3S.jpg" data-fancybox>
	<img src="https://i.imgur.com/SGtZS3S.jpg" alt="" />
</a></center>

As stated above, I did a decent amount of damage to the donor PCBs when I removed them from the Advantage. I needed a total of **9** patch wires to get the PCBs functional again. It's been ages since I've needed to patch a circuit board - I think the last time was my very first keyboard, an Alps64. This patch work proved to be quite challenging. The matrix on the Kinesis aren't laid out like any other keyboard I've worked with, and with no reference material or spare PCBs to inspect, it took a lot of trial and error to get the first keywell functional. The second keywell was a lot easier as I took photos of both sides of the PCB _before_ I soldered it into place. The lesson learned is that I shouldn't try to wing repairs when I know they'll be necessary. Any future projects that I go into know I'll need to perform repairs - I'll document prior to soldering anything in place.

The last step in this process was to solder in new switches on the thumb clusters. These little PCBs are just like standard PCBs, so the process was quick and painless.

Going into the work on Sunday, I'd really hoped to get the project _complete_, alas - complex tasks always take longer than you think. I won't have time for another marathon 8 hour soldering session this week, so I imagine completion will need to wait until next weekend. In the interim I'll be working on getting RGB LED functionality up and running in the Stapleberg's QMK firmware.

Once the project is complete, I'll have a video up on my YouTube channel as well. Stay tuned for more on this!

Next: [Kinesis Reloaded: Day 2]({{ site.baseurl }}/keyboards/2018-02-13-Kinesis-Reloaded-Day-2)

---
<p align="right">Typed on Blue Alps64</p>
