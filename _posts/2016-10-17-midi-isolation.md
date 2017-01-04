---
title: Optical isolation via MIDI
---
Here is the current setup, wherein I am attempting to isolate the sensor and microcontroller from the computer with
a midi breakout board and a midi box on the other end. The theory is that since midi is [optically isolated by
contract](https://www.midi.org/specifications/item/midi-din-electrical-specification) the computer's noisy ground
plane will no longer be a problem. 

![midi boards and box]({{ site.url }}/images/DSC_0399.JPG)

Unfortunately, this did not work. Apparently, the length of the midi cable itself acts as enough of an antenna to
introduce noise into the system (!). When the cable is plugged in, the ECG board will not read, and when unplugged
it picks up my heartbeat just fine. Maddening, yes, but at this point also borderline hilarious.

I would try optically isolating the Olimex board's serial port, but it is hardwired to 115200 baud, which is faster than
any optical isolators support. Instead, I am going to try [this weird-ass digital isolator
chip](http://www.silabs.com/products/power/isolators/Pages/Si86xx-Digital-Isolators.aspx). The datasheet says it is
capable of 2mbps data transmission, which is more than enough.
