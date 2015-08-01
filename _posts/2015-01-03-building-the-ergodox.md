---
layout: project
title:  "So I tried to make an Ergodox ..."
date:   2015-1-3 13:58:44
categories: keyboards
seqprevious: /keyboards/2014/10/05/sourcing-the-ergodox/
seqnext: /keyboards/2015/06/29/ergodox-update/
---

So, you'll notice in this has had a substancial amount of time since the last time I posted about the keyboard... Sufice to say, things didn't go that well. At any rate, and I'll tell you my pitfalls and where I plan on going from here!

#### Where I'm at now
So I soldered everything together and only half of the keyboard works. I can get the half with the teensy to work just fine, but the other side does nothing. It looks pretty nice, the wood case came out pretty great, but I think that I need to make some changes so that it sits at a good angle. I still want to change up the case so that it: A) uses plastic on part, B) includes a wrist rest, and C) is angled like my ms sculpt.

#### Pitfalls of an amature and inexperienced solderer
So, hand soldering surface mounted diodes == bad times. I did this. With tweezers and a soldering iron and LOTS of patience. I didn't really know how the surface mounted thing worked. Now I do and I wish I hadn't tried to do it. I have enough space in my case that I easily could have used the through hole diodes. Probably things would have worked better if I had done that. 

My advice: if you don't know how to solder surface mounted chips and haven't done it before, don't make this your first project where you try it. Just go with the through hole diodes.  You'll have much less pain doing it and you're way less likely to screw it up. If you really want surface mounted ones, go get some prototyping boards and do some tests first.

#### MCP23018-E/SP-ND != MCP23017-E/SP-ND
These are not the same thing. I made that mistake. Digikey was out of the 18 and so I thought, "Hey, they're both I2C expanders. I'll just get the other one." It did fit in the holes, which probably made it worse, but sufice to say, my solder removal skills have greatly improved as a part of this project. Not enough that I didn't destroy my pcb while I was trying to do it. Also, while were at it Dremels cannot solve all probems. I thought maybe they could, I was pretty wrong about that.

To make matters worse, when I went and ordered the 18, I accidentally ordered the non-I2C version, which also totally doesn't work. Soldered that one on too before I realized my mistake. Suffice to say I melted the heck out that pcb with my clumsy soldering iron hands before I tried to put the right one on. Hence needing to order another one.

#### The case works...
![Soldering Iron]({{site.baseurl}}/images/ergodox/ergodox-case.jpg) 
One thing that did work was the case, the laser cut through the wood like butter and it fit together pretty well. I did have to do the conversions from dxf to svg which turned out to be more difficult than I expected on a mac. The end result looks pretty cool. I'm certainly going to go through and make the case really different. I didn't realize how relient I am on the wrist rest on my sculpt, but I thought about it the other day and I think I'll be pretty miserable without one.
![Soldering Iron]({{site.baseurl}}/images/ergodox/laser-cutting.jpg) 

I can't take credit for all of that design, I did the flying saucer and the beam and the stars, but my [wife](http://courtneygives.github.io) did the exploding planet for me.

#### Where I'm going next
I've clearly abandoned this project for several months. Now that some of my wounded pride has worn off, I'm going to try and finish it. And by finish it, I mean, I'm going to start the left hand again from scratch with a new PCB. Right now, [Mechanical Keyboards](http://mechanicalkeyboards.com/shop/index.php?l=product_detail&p=537) is out of stock on the pcb's and I'm feeling a little too lazy to have them fabbed anywhere. So I'll wait patiently for them to come back in stock and order another set. I'm beginning to approach the cost of the massdrop kit, so that has me a bit bummed. In the mean time, I did manage to pull the key off the right half of my space bar on my microsoft sculpt and fix it without breaking it. So that's a plus. I'm still using the sculpt and I think I still like it okay, but I'm sad that I don't have an ergodox at my desk right now.