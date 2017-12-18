---
layout: page
title: "Brown Alps Iris Build Log"
subheadline: ""
teaser: ""
author: Morgan
categories:
  - keyboards
image:
    title: https://imgur.com/OMq4LMR.jpg
    homepage: https://imgur.com/OMq4LMR.jpg
    thumb: https://imgur.com/OMq4LMR.jpg
    caption:
    caption_url:
breadcrumb: true
comments: true
---

The [Iris](https://keeb.io/collections/split-keyboard-parts/products/iris-keyboard-split-ergonomic-keyboard) ergonomic split keyboard first appeared on my radar in September, when [u/Bakingpy](https://www.reddit.com/user/bakingpy) of [Keeb.io](https://keeb.io/) posted a picture of the first [Iris prototype](https://www.reddit.com/r/MechanicalKeyboards/comments/6yfhdv/photos_finished_the_very_first_half_of_an_iris/) on [r/mk](https://www.reddit.com/r/MechanicalKeyboards/). Since building my test [ErgoDox]({{ site.baseurl }}/2016-07-18-ErgoDox-Build-Phase-III-Testing)  I've taken a serious interest in split keyboards, and was actively on the hunt for another split board. Most of the selection out there like [Let's Split](https://github.com/nicinabox/lets-split-guide) and [Orthodox](https://geekhack.org/index.php?topic=89279.0) are based on the [40%](https://deskthority.net/wiki/40%25) layout, as opposed to the [60%](https://deskthority.net/wiki/60%25) layout. While innovative and filling a niche, I find the 40% footprint to have too few keys for me, so something based on a 60% was what I was after.

Prior to seeing Iris, I'd taken an interest in the [Dark Matter](https://hackaday.com/tag/dark-matter-keyboard/) split keyboard. While 40% based, I loved the look, and had started some tentative plans to design and build my own custom split board. I even ordered [MT3](https://matt3o.com/about-mt3-profile-and-devtty-set/) keycaps to fit my hypothetical board. What caught my eye about Iris is its layout. Iris is laid out almost _identical_ to the split board idea I'd been toying with. I knew as soon as I saw it that I had to have one.

<center>
<a href="https://imgur.com/e30JINB.jpg" data-fancybox>
	<img src="https://imgur.com/e30JINB.jpg" alt="" />
</a></center>

Iris uses the same column stagger that ErgoDox does. It omits the inner 1.5u keys and most of the thumb cluster, opting for a single thumb key as opposed to the two side-by-side thumb keys on ErgoDox. Iris' firmware and pin out are based on Keeb.io's [NyQuist](https://keeb.io/products/nyquist-keyboard?variant=48309345990) split keyboard (another ortholinear split board), which is in turn based on Let's Split. Iris also supports RGB underglow, LED backlighting, and can use MX or Alps switches. Pricing for Iris is extremely budget friendly - the PCBs, controllers, and case are just $70 combined. Significantly cheaper than the $100+ one would pay to get started on an ErgoDox. This board is actually inexpensive enough that I ended up ordering two!


## The Parts

+ 2x White Iris PCBs
+ 2x White PCB material plates
+ 54x diodes
+ 54x Brown Alps Switches
+ 2x Arduino Pro Micros
+ OnePerDesk Alps keycaps

### The PCBs & Plates

<center>
<a href="https://imgur.com/Vf4kndZ.jpg" data-fancybox>
	<img src="https://imgur.com/Vf4kndZ.jpg" alt="" />
</a></center>

At launch, Iris was available with black, white, or blue PCBs. Cases were available in black PCB material or white acrylic. There's been a trend lately of folks using PCB material for keyboard plates (popularized by the Mitosis keyboard). PCB material is great, it's nearly as strong as metal plates, but at acrylic plate pricing. While white material plates were not offered at launch, I was able to score a set from Keeb.io out of the remainders of prototype plates. I love the contrast between the white plates and brown keycaps - it really makes this board pop.

### The Switches

<center>
<a href="https://imgur.com/rsM5rRN.jpg" data-fancybox>
	<img src="https://imgur.com/rsM5rRN.jpg" alt="" />
</a></center>

For the white Iris build I saw an opportunity to finally make use of a set of [Brown Alps](https://deskthority.net/wiki/Alps_SKCM_Brown) switches I'd been holding on to for over a year. To my knowledge brown alps were only ever in the IBM 5150 and Magnavox VideoWriter keyboards. When I bought them, they were still soldered to the 5150 keyboard. I bought the board without any specific project in mind, but I'm very glad that I did. They're a lovely heavy tactile switch, with a strong, crisp tactile bump right at the top. They feel fantastic and might be my new favorite Alps switch; I'm glad to have finally had the chance to use them on something.

### The Keycaps

<a href="https://imgur.com/AUULy5j.jpg" data-fancybox>
	<img src="https://imgur.com/AUULy5j.jpg" alt="" />
</a>

In keeping with my other Alps build ([white]({{ site.baseurl }}//keyboards/2016-02-24-1-White-Alps-Build-Log) and [blue]({{ site.baseurl }}/keyboards/2016-04-04-Blue-Alps-Build-Log)), this board has keycaps that match the switches underneath them. With brown alps switches it's only natural to use brown keycaps. I scored these on [r/mechmarket](https://www.reddit.com/r/mechmarket/) _after_ I ordered the Iris parts, so the timing was perfect.

These keycaps are from the [One Per Desk](https://deskthority.net/wiki/ICL_One_Per_Desk) computer keyboard. The board these come from actually isn't mechanical, it uses sliders over membrane, fortunately these are still compatible with Alps switches. If the brown + red colorway seems familiar, you may recognize it from [SA Retro](https://ctrlalt.io/buys/sa-retro). As it turns out, the One Per Desk served as the inspiration for _that_ keycap set.




## Assembly


<div class="video-container"><iframe title="YouTube video player" class="youtube-player" type="text/html"
width="640" height="390" src="http://www.youtube.com/embed/aZQpGw9KoQE"
frameborder="0" allowFullScreen></iframe></div>

For this build, I used a [PCB holder](http://amzn.to/2BBAHPA) for the first time. I've seen them on other build logs and have meant to buy one for a long time. The holder was a god-send for this build, and greatly simplified the process.

<center><ul class="clearing-thumbs small-block-grid-4" data-clearing>
  <li><a href="https://i.imgur.com/unsUItd.jpg"><img data-caption="" src="https://i.imgur.com/unsUItd.jpg"></a></li>
  <li><a href="https://imgur.com/s4oXK0j.jpg"><img data-caption="" src="https://imgur.com/s4oXK0j.jpg"></a></li>
  <li><a href="https://imgur.com/eCIdCCW.jpg"><img data-caption="" src="https://imgur.com/eCIdCCW.jpg"></a></li>  
</ul></center>

Assembly of Iris begins with soldering on diodes. Diodes are what gives a keyboard matrix n-key rollover. Diodes install on one side of the board, and are soldered on the other. I typically tape diodes down during soldering so that they don't fall out.

<center><a href="https://imgur.com/RVgMX5e.jpg" data-fancybox>
	<img src="https://imgur.com/RVgMX5e.jpg" alt="" />
</a></center>

After soldering diodes, headers for the [Pro Micros](https://www.sparkfun.com/products/12640) are installed, along with a right-angle reset switch and TRRS jacks. Iris uses common TRRS cables over serial to connect the two halves.

After the somewhat tedious task of prepping the PCBs, it's time to solder on switches.

<center>
<a href="https://imgur.com/YyU5YtH.jpg" data-fancybox>
	<img src="https://imgur.com/YyU5YtH.jpg" alt="" />
</a></center>

Following switches, it's time to solder on the Pro Micros. Note: during the initial build of this board I soldered both Pro Micros on with the same orientation. Desoldering a Pro Micro is a big pain. Don't make the same mistake I did. Be sure to solder on the Pro Micro on the left with components up, and the right side with components down.

<a href="https://imgur.com/RoAAjRb.jpg" data-fancybox>
	<img src="https://imgur.com/RoAAjRb.jpg" alt="" />
</a>

With control electronics soldered on, the last (optional) step of assembly was to add RGB LED strips to each hand. The Iris PCBs were designed with RGB underglow in mind. Previous boards I've build with RGBs have involved soldering directly to pins on a controller chip, this PCB has dedicated pinouts on each hand, greatly simplifying the process.

<center>
<a href="https://imgur.com/6tbgHiU.jpg" data-fancybox>
	<img src="https://imgur.com/6tbgHiU.jpg" alt="" />
</a></center>

Lastly I assembled the case, and assembly was done.


## The Code

Iris runs on [QMK](http://qmk.fm/), my keyboard firmware of choice. The keymap files have been merged into the main QMK repository and are available [here](https://github.com/qmk/qmk_firmware/tree/master/keyboards/iris).

I had a small learning curve while building my keymap for Iris. It had been nearly a year since I'd build a QMK-based keyboard, so **many** things had changed and improved. QMK now supports arbitrary custom keycodes. With arbitrary keycodes you can keep a keymap cleaner and easier to read, and define function layers and macros much easier. In the past it was necessary to have a function inline in the keymap, like:

```c
FN1
```

then define it with something like after the keymap with all the other function keys, like:

```c
const uint16_t PROGMEM fn_actions[] = {
    [1]  = ACTION_LAYER_TAP_KEY(1, KC_SPC),
```

Now, you can have really simple definitions above you keymap, then drop the arbitray keycode into the keymap.

As an example, I can define a simple dual role function key (backspace when tapped, function key when held) with:

```c
#define KC_BSLR LT(_LOWER,KC_BSPC)
```
then just use the keycode
```c
BSLR
```
_inside_ my keymap

 With its new build environment, flashing a keyboard is now far simpler and easier - especially for boards that use a Pro Micro. In the past it was necessary to compile your firmware, then plug in a promicro, trigger it's reset mode, quickly find its COM port, then flash the firmware using another utility. Now one runs a simple command and QMK compiles & flashes the board in one step. For Iris the command is ```make iris/rev2:default:avrdude```

 My Iris keymap is below. Mostly an adaptation of my ErgoDox keymap, combine with how I typically lay out my 60% boards.

```c
#define _QWERTY 0
#define _LOWER 1
#define _RAISE 2
#define _ADJUST 16

enum custom_keycodes {
  QWERTY = SAFE_RANGE,
  LOWER,
  RAISE,
  ADJUST,
};

#define KC_ KC_TRNS
#define _____ KC_TRNS

#define KC_LOWR LOWER
#define KC_RASE RAISE
#define KC_RST RESET
#define KC_BL_S BL_STEP

#define KC_CLCA CTL_T(KC_CAPS)
#define KC_SPLR LT(_LOWER,KC_SPC)
#define KC_BSLR LT(_LOWER,KC_BSPC)

#define KC_MHME LGUI(KC_LEFT)
#define KC_MEND LGUI(KC_RGHT)

const uint16_t PROGMEM keymaps[][MATRIX_ROWS][MATRIX_COLS] = {

  [_QWERTY] = KC_KEYMAP(
  //,----+----+----+----+----+----.              ,----+----+----+----+----+----.
     EQL , 1  , 2  , 3  , 4  , 5  ,                6  , 7  , 8  , 9  , 0  ,MINS,
  //|----+----+----+----+----+----|              |----+----+----+----+----+----|
     TAB , Q  , W  , E  , R  , T  ,                Y  , U  , I  , O  , P  ,BSLS,
  //|----+----+----+----+----+----|              |----+----+----+----+----+----|
     LCTL, A  , S  , D  , F  , G  ,                H  , J  , K  , L  ,SCLN,QUOT,
  //|----+----+----+----+----+----+----.    ,----|----+----+----+----+----+----|
     LSFT, Z  , X  , C  , V  , B  ,BSLR ,    SPLR , N  , M  ,COMM,DOT ,SLSH,RSFT,
  //`----+----+----+--+-+----+----+----/    \----+----+----+----+----+----+----'
                       LALT,LGUI,BSLR ,        SPLR ,ENT ,DEL
  //                  `----+----+----'        `----+----+----'
  ),

  [_LOWER] = KC_KEYMAP(
  //,----+----+----+----+----+----.              ,----+----+----+----+----+----.
     ESC ,MUTE,VOLD,VOLU,MPRV,MPLY,               MNXT,    ,    ,SLSH,BSPC,    ,
  //|----+----+----+----+----+----|              |----+----+----+----+----+----|
         ,    , UP ,    ,MHME,MEND,               LBRC,  7 ,  8 ,  9 ,MINS,    ,
  //|----+----+----+----+----+----|              |----+----+----+----+----+----|
     CAPS,LEFT,DOWN,RGHT,HOME, END,               RBRC,  4 ,  5 ,  6 ,PLUS,    ,
  //|----+----+----+----+----+----+----.    ,----|----+----+----+----+----+----|
      RASE,    ,    ,    , SPC, ENT,TRNS,     TRNS, F13 ,  1 ,  2 ,  3 ,ENT ,GRV,
  //`----+----+----+--+-+----+----+----/    \----+----+----+----+----+----+----'
                           ,    ,TRNS,         TRNS,  0 , DOT
  //                  `----+----+----'        `----+----+----'
  ),

  [_RAISE] = KC_KEYMAP(
  //,----+----+----+----+----+----.              ,----+----+----+----+----+----.
     F12 , F1 , F2 , F3 , F4 , F5 ,                F6 , F7 , F8 , F9 ,F10 ,F11 ,
  //|----+----+----+----+----+----|              |----+----+----+----+----+----|
         ,    ,  Q ,    ,    ,    ,                   ,    ,    ,    ,   ,    ,
  //|----+----+----+----+----+----|              |----+----+----+----+----+----|
         ,    ,    ,    ,    ,    ,                   ,    ,    ,    ,    ,    ,
  //|----+----+----+----+----+----+----.    ,----|----+----+----+----+----+----|
    RASE ,    ,    ,    ,    ,    ,    ,         ,    ,    ,    ,    ,    ,    ,
  //`----+----+----+--+-+----+----+----/    \----+----+----+----+----+----+----'
                           ,    ,    ,             ,    ,
  //                  `----+----+----'        `----+----+----'
  ),

  [_ADJUST] = KEYMAP(
  //,--------+--------+--------+--------+--------+--------.                          ,--------+--------+--------+--------+--------+--------.
      _____, _____, _____, _____, _____, _____,                            _____, _____, _____, _____, _____, _____,
  //|--------+--------+--------+--------+--------+--------|                          |--------+--------+--------+--------+--------+--------|
      RGB_TOG, RGB_MOD, RGB_HUI, RGB_SAI, RGB_VAI, _____,                            _____, _____, _____, _____, _____, _____,
  //|--------+--------+--------+--------+--------+--------|                          |--------+--------+--------+--------+--------+--------|
      RESET  , DEBUG  , RGB_HUD, RGB_SAD, RGB_VAD, _____,                            _____, _____, _____, _____, _____, _____,
  //|--------+--------+--------+--------+--------+--------+--------.        ,--------|--------+--------+--------+--------+--------+--------|
      BL_STEP, _____, _____, _____, _____, _____, _____,          _____, _____, _____, _____, _____, _____, _____,
  //`--------+--------+--------+----+---+--------+--------+--------/        \--------+--------+--------+---+----+--------+--------+--------'
                                      _____, _____, _____,                  _____, _____, _____
  //                                `--------+--------+--------'                `--------+--------+--------'
  )

};
```

## The Result

<center>
<a href="https://imgur.com/pCWcKds.jpg" data-fancybox>
	<img src="https://imgur.com/pCWcKds.jpg" alt="" />
</a></center>

I've been really quite pleased with this board. It's my first split since my test ErgoDox. I love the look, I love how compact yet functional it is. While Iris has fewer keys than ErgoDox, I find it nearly as productive. There's a LOT of functionality baked into such a small board.

I've been daily driving it at work for a month or so now and have been loving it. The brown alps switches are just glorious. The keycaps feel great, and I love just _looking_ at the thing.

<center><ul class="clearing-thumbs small-block-grid-4" data-clearing>
  <li><a href="https://imgur.com/rINM5xg.jpg"><img data-caption="" src="https://imgur.com/rINM5xg.jpg"></a></li>
  <li><a href="https://imgur.com/AUULy5j.jpg"><img data-caption="" src="https://imgur.com/AUULy5j.jpg"></a></li>
  <li><a href="https://imgur.com/lXlN5Uq.jpg"><img data-caption="" src="https://imgur.com/lXlN5Uq.jpg"></a></li>
  <li><a href="https://imgur.com/RH5Au35.jpg"><img data-caption="" src="https://imgur.com/RH5Au35.jpg"></a></li>      
</ul></center>
https://imgur.com/rINM5xg.jpg
Coming soon I'll have another Iris build (as soon as keycaps arrive) - the next one will use a black case, [Otemu Ice](https://www.novelkeys.xyz/product/outemu-ice-switches/) switches, and Russian MT3 keycaps. Stay tuned!





---
<p align="right">Typed on Brown Alps Iris</p>
