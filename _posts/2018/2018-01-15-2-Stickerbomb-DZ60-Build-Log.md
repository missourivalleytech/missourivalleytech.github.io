---
layout: page
title: "Stickerbomb DZ60 HHKB Build Log"
subheadline: ""
teaser: "I loved the look of the stickerbombed case, but not the layout. I'm firmly a 60% guy, I simply didn't have interest in a TKL layout board. I knew that to make one for myself, and to have the HHKB layout I love, I'd have to endeavor to build my first truly custom keyboard case."
author: Morgan
categories:
  - keyboards
image:
    title: https://imgur.com/sALsXma.jpg
    homepage: https://imgur.com/sALsXma.jpg
    thumb: https://imgur.com/bVUnqAh.jpg
    caption:
    caption_url:
breadcrumb: true
comments: true
---

About a year ago, I noticed a product on [1UpKeyboards](https://1upkeyboards.com/diy-tkl-2-plate-ss-sticker-kit.html) for a stickerbomb TKL layout keyboard. The kit on the site offered two metal plates and a pack of stickers. Prior to the stickerbomb TKL launch, I'd seen plenty of stickerbombed keyboards, usually folks slapping stickers on existing cases. I really fell in love with the TKL on 1UpKeyboards because it used a skeleton/sandwich design, a case made of just two plates. I loved the raw look of it, the pictures on the site looked more three dimensional that other stickerbomb boards I'd seen. It looked more _interesting_, it had depth, because you could see stickers on both plates, as opposed to just stickers slapped on a standard plastic case.

I loved the _look_ of the case, but not the layout. When it comes to standard staggered keyboards, I'm firmly a 60% guy. I simply have no interest in a TKL layout keyboard. Sadly, 1Up did not (and to date has not) offered a similar product in a 60% layout. I knew that to make one for myself, I'd have to endeavor to do my first **truly** custom keyboard case. I started doing research on how to have a custom plate made, and how to design one.

### The Case

<center>
<a href="https://imgur.com/aixKgw3.jpg" data-fancybox>
	<img src="https://imgur.com/aixKgw3.jpg" alt="" />
</a></center>

Getting ready to design the plates, I settled on what I wanted out of the case. My big priorities were for a [HHKB](https://en.wikipedia.org/wiki/Happy_Hacking_Keyboard) layout, with wide bezels, and support for split-spacebars. I knew going into the design that I would be putting stickers all over the plates, so I wanted as much space as possible to highlight the stickers. The wide bezel all the way around allows more stickers to be seen, and the blocked off keys on the bottom row would give me even more room to feature stickers. I also chose the HHKB layout because it's simply my favorite arrangement for 60% keyboards. I've already got a board with this layout, and love using it.

To design the board, I first mocked up a design on [Keyboard Layout Editor](http://www.keyboard-layout-editor.com/), then copied the raw data from KLE into [Swill's Plate Builder](http://builder.swillkb.com/) tool. If you haven't used Swill's tool before, it's amazing. Without this tool I likely would never have had the ambition to do this build. Swill's tool imports the raw layout data from KLE, and provides a SVG or DWF output with a plate design. There are tons of levers and switches on the site - you're able to adjust the plate design for use in standard 60% cases or sandwich & skeleton style cases (like this build), adjust the screw hole size, bezel, corner radius, and more!

![](https://imgur.com/iQGXhSJ.jpg)

The output from Swill's tool gave me a good basis for the plate design. From there I made further adjustments to the design using [QCad](https://qcad.org/en/). Specifically I made adjustments to the stabilizer openings, and switch openings for the split spacebar. Designs for the case are available here.

For manufacture, I opted to use [Ponoko](https://www.ponoko.com/). There are also a bunch of other companies that can do custom-cut plates. For acrylics, [Sculpteo](https://www.sculpteo.com/en/), for metals, [BigBlueSaw](http://www.bigbluesaw.com/). The plates I ordered from Ponoko were 1.5mm clear acrylic. In hindsight, I likely should have ordered thicker plates. By themselves the 1.5mm plates were quite flimsy - this had been a hand wired build they would've been completely unsuitable. Fortunately, once fully assembled the board was quite sturdy, but if I could do it over again, I likely would've ordered 3mm acrylic, or opted for steel plates.

### PCB

<center>
<a href="https://imgur.com/vVGwyHo.jpg" data-fancybox>
	<img src="https://imgur.com/vVGwyHo.jpg" alt="" />
</a></center>


Aside from the case, all other parts for this build use off-the shelf parts. While this is not my first 60% layout board, this was my first time using the [DZ60 PCB ](https://kbdfans.myshopify.com/products/dz60-60-pcb) from KBDFans. I've been really impressed with this circuit board. It's available at a **very** competitive price, just $40. It has integrated RGB underglow, runs on [QMK](http://qmk.fm/), supports LED backlighting, works with all standard [POKER](https://deskthority.net/wiki/Vortex_Pok3r) style 60% keyboard cases, and is compatible with more layouts than any other circuit board I'm aware of. The killer for this PCB is its bottom row - with support for 6u, 6.25u, 7u, and split spacebars. I plan on using the DZ60 for the next few 60% builds I have planned.

### Stickers

<center>
<a href="https://imgur.com/gZb241r.jpg" data-fancybox>
	<img src="https://imgur.com/gZb241r.jpg" alt="" />
</a></center>

As I refined more ideas about how to execute this build, I decided that I wanted a 'theme' for the stickers. I already had a couple sticker packs, and was gifted a [Rick and Morty stickerpack](http://amzn.to/2r0wjpg) by my girlfriend. As a big fan of the show, I opted to use a Rick and Morty theme for this build. The majority of the visible stickers are from the Rick and Morty pack, and I set the RGB underglow on the PCB to green - a la the green of Rick's portal gun.

# The Build

<div class="video-responsive">
    <iframe width="640" height="360" src="http://www.youtube.com/embed/C5t-wfHaxUs" frameborder="0" allowfullscreen></iframe>
</div>

All parts for this build:

+ Custom plates
+ DZ60 PCB
+ Zealio 78g switches
+ Gateron black switches
+ Plate mount stabilizers
+ Maxkey SA Ninja keycaps
+ Assorted stickerbomb pack
+ Rick and Morty sticker pack
+ Knurled M3 spacers and hex M3 screws

This build was one of my longer ones. A lot of keyboards I can build in just a couple hours; assembly for this build took over 6. I started by prepping the plates. First, the protective cover over the acrylic was removed. Then I started applying stickers over both plate until they were fully covered. Then came the process of cutting out switch holes in the top plate. This initial prep took well over two and a half hours.

<center>
<a href="https://imgur.com/RtNXFFW.jpg" data-fancybox>
	<img src="https://imgur.com/RtNXFFW.jpg" alt="" />
</a></center>

After I was satisfied with stickers on the plate, I applied a Rustoleom clear enamel on both top and bottom plates, so that the stickers would stay down on the acrylic, and be protected from bumps and scratches.

While the enamel dried I prepped my stabilizers. As I've done before, I clipped the stabilizer legs and used [Finish Line Extreme Flouro](http://amzn.to/2D3lIvj) lube. New (to me) for this build was the band aid mod. With this mod, sections of cloth band aids are cut up and applied on the PCB, below the stabilizers. This mod reduces stabilizer rattle significantly, and provides a very slight cushion when stabilized keys are fully depressed. With all these mods and work, I can say conclusively that this board has the best feeling stabilizers I've ever used.

Once the enamel dried, it was time to install switches. Here the thin plates hurt me. With how flexible the top plate is, it took a lot of effort to get the switches fully seated in the plate and on the PCB. If I'd chosen a thicker acrylic or stronger material, this would have been a much simpler process.

<center>
<a href="https://imgur.com/AeCJcv0.jpg" data-fancybox>
	<img src="https://imgur.com/AeCJcv0.jpg" alt="" />
</a></center>

The primary switches for this build are 78g Zealio switches. I've done boards with Zealios before, but never this heavy. As I've gotten deeper and deeper into this hobby, I've gained a big appreciation for heavy switches. These Zealios feel excellent. They're smooth, tactile, and heavy, but not too heavy. I also installed Gateron blacks for the shift keys and spacebar. I like my shift and spacebars to be lighter than my alphas, and linear. These Gateron blacks are great, a big upgrade over the Cherry blacks I've used previously. The Gaterons have a similar weight as the Cherrys, but are significantly smoother.

With switches installed, I broke out my handy circuit board holder and began soldering.

<center>
<a href="https://imgur.com/VMGf3WM.jpg" data-fancybox>
	<img src="https://imgur.com/VMGf3WM.jpg" alt="" />
</a></center>

Now that soldering was complete, I assembled the board, installed keycaps, and got to programming.

### Spacebars

<center>
<a href="https://imgur.com/pMx1Ndo.jpg" data-fancybox>
	<img src="https://imgur.com/pMx1Ndo.jpg" alt="" />
</a></center>

Friends I've showed this board to have asked me what split spacebars achieves. If you're like my, you tend to hit your space bar using only one hand, and usually in the same spot every time. If you're hitting the a very limited part of the spacebar regularly, that means a lot of space is being wasted. I learned to appreciate having multiple functions for what a thumb key could do when I built my [ErgoDox]({{ site.baseurl }}/ErgoDox_Omnibus), and later [Iris]({{ site.baseurl }}/keyboards/2017-12-18-2-Brown-Alps-Iris-Build-Log). I love having space for my right thumb, and backspace for my left thumb - that's exactly how this board is laid out. From left to right the bottom row does this:

``` ALT | CMD | Backspace | Enter/FN | Space/FN | CMD | ALT ```

The full keymap file for this board is available [here]({{ site.baseurl }}/Files/Keyboards/Stickerbomb_DZ60/keymap.c).

# Final Thoughts

<center><ul class="clearing-thumbs small-block-grid-4" data-clearing>
  <li><a href="https://imgur.com/sALsXma.jpg"><img data-caption="" src="https://imgur.com/sALsXma.jpg"></a></li>
  <li><a href="https://imgur.com/BH8sDn6.jpg"><img data-caption="" src="https://imgur.com/BH8sDn6.jpg"></a></li>
  <li><a href="https://imgur.com/Fnzl8l1.jpg"><img data-caption="" src="https://imgur.com/Fnzl8l1.jpg"></a></li>
  <li><a href="https://imgur.com/N5Mjj95.jpg"><img data-caption="" src="https://imgur.com/N5Mjj95.jpg"></a></li>      
</ul></center>

This board took a lot of time and effort to put together. I had been toying with, working on, and acquiring parts for this build for over a year. Given all the **true** custom work needed to build this board, I have a lot of pride in this build. There were a few missteps along the way (mostly with my plate material choice), but despite those missteps this board turned out better than I could have imagined. This stickerbombed DZ60 feels great to type on, and is visually very striking. It's far from a 'clean' looking build, but it wasn't meant to be. This board was meant to be loud, and gaudy, and over the top - and it is.


---
<p align="right">Typed on Stickerbomb DZ60</p>
