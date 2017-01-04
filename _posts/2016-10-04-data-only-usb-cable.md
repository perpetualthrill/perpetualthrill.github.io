---
title: Attempting to solve noise with data-only USB
---
In an effort to make sure the microprocessor and ECG boards do not receive noisy USB power, I made this terrible thing --
a USB cable with the power wire physically cut. Unfortunately, while data transfer is successful, the setup was still
too noisy, which surprised me.

I take this to mean that the common ground shared between USB and the batteries is where the noise is coming from. It's 
frustrating, particularly given that USB isolators start at like fifty bucks. Also, given that the noise is low-frequency
(otherwise the op-amps on the Olimex board would catch it) an RF choke is not useful here.

![usb cable hack]({{ site.url }}/images/data-only-usb.jpg)
