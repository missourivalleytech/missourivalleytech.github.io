---
layout: page
title: "The Stapleberg Controller"
subheadline: ""
teaser: "The Stapleberg controller is a QMK-compatible drop-in replacement control electronics for Kinesis Advantage keyboards."
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

<center>
<a href="https://imgur.com/EIQ8fod.jpg" data-fancybox>
	<img src="https://imgur.com/EIQ8fod.jpg" alt="" />
</a></center>

Today I received the [Stapleberg controller](https://michael.stapelberg.de/Artikel/kinesis_custom_controller) (and associated electronics) from a recent [group buy](https://www.reddit.com/r/mechmarket/comments/78r605/gb_kinesis_qmk_mod_kit_using_stapelberg/) on Reddit.

The Stapleberg PCB is a drop-in replacement for the control electronics in modern [Kinesis Advantage](https://www.kinesis-ergo.com/shop/advantage2/) keyboards. While Kinesis boards have some level of on-board programming ability by default from the factory, the default programming options aren't nearly as flexible as my favorite keyboard firmware: [QMK](http://qmk.fm/).

Designed by [Michael Stapleberg](https://michael.stapelberg.de/), this controller provides an easy way to control a Kinesis Advantage using a [Teensy++](https://www.pjrc.com/store/teensypp.html) development board. His custom-designed PCB connects the Kinesis' existing circuit boards to the Teensy. As a result of his work and reverse engineering of the Kinesis key matrix, it's no longer necessary to hand wire connections to the various matrix boards inside the Advantage keyboard.

<center>
<a href="https://imgur.com/9pCXqKb.jpg" data-fancybox>
	<img src="https://imgur.com/9pCXqKb.jpg" alt="" />
</a></center>

I've long been fascinated with Kinesis Advantage keyboards, since before I was even a keyboard wonk. I remember first seeing them in [Men In Black](https://deskthority.net/wiki/Kinesis_Contoured#Trivia), noting how out-of-this-world they seemed. In [February]({{ site.baseurl }}/keyboards/2017-02-09-Kinesis-Countoured-Model-110) last year, I got my hands on a Kinesis Contoured [Model 110](https://deskthority.net/wiki/Kinesis_Contoured#Model_100) (pictured above). The Model 110 (circa 1991) is visually very similar to the modern-day Advantage boards, but its internals are significantly different. I do believe the cases are identical, however the keywell and thumb cluster PCBs aren't the same in any way.

I bought this Stapleberg controller with the intent of using it to modernize my Model 110. As it turns out, the Stapleberg is only compatible with modern Advantage style keywell and thumb cluster PCBs, so I will need to source all new internals for my Model 110 - this isn't a big deal though as my Model 110 isn't fully functional anyway.

In order to complete this rebuild, I'll likely need to replace every single internal component in my Model 110, but the result will be a fully modern, fully programmable keyboard.

---
<p align="right">Typed on Dasher & Dancer DZ60</p>
