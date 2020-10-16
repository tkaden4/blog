---
layout: post
title: "Making a PLC Training Board, Pt. 1"
---

Programmable logic controllers, also known as PLCs, are widely used for industrial automation. I tend to think of them as an industrial-strength arduino,
since they are built to handle rougher environments, and often have preloaded algorithms for PID, which is common in control loops.

I wanted to get some experience with these devices as soon as possible, as it is closest to the work I have done before in software development, although
the programming languages used for PLCs are quite foreign to me.

## Choice of PLC - CLICK C0-00DD2-D

<img src="https://cdn.automationdirect.com/images/products/large/l_c000dd2d.jpg" style="max-height: 400px">

I chose the Koyo CLICK C0-00DD2-D as my PLC for a couple reasons:

- It's cheap, with a cost of \$69 on AutomationDirect
- It was recommended by my textbook for Instrumentation
- The programming software was free

I also purchased the optional 24VDC power supply for \$40, as it was more convenient than hooking up my
bench supply to the PLC every time I wanted to use it.

<img src="https://cdn.automationdirect.com/images/products/large/l_c001ac.jpg" style="max-height: 400px">

## The Board

<img src="{{ site.baseurl }}/assets/plc/plc-board.jpg" style="max-height: 400px">

This is what the finished board looks like. The components are all mounted on
four different DIN rails that I was able to get in bulk off of ebay for under \$20.
On top we have a breaker so that I can conveniently switch power on and off to the
24VDC power supply, as well as providing some overcurrent protection.

On the bottom we have the PLC with the power supply, and some terminal blocks for
wiring convenience.

<img src="{{ site.baseurl }}/assets/plc/plc-stand.jpg" style="max-height: 600px">

This is the board from the back. I cut up parts from an old chair my roommates were
throwing out to make the stand for the board, to keep the bolts holding the rails
on from scratching whatever surface I put it on.

## Next Steps

While this is a good start to a PLC board, there are a few improvements I would like to make:

- Adding an HMI (Human-Machine Interface), probably a touch panel
- Getting an analog input/output board, so that I can practice more with 4-20mA loops
- Installing some basic discrete input and output elements, such as LEDs and pushbutton switches

In part two, I will show some simple ladder logic programs and install the discrete input/output elements
I mentioned above.
