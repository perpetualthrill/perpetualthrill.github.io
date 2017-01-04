---
title: Rebuilt proto with Olimex ECG board and external power supply
---
Actually, I tried three different power supplies, and all of them seem to be too noisy for the Olimex board. Which
is too bad, because it outputs a one-byte ECG reading over UART, which fits our processing needs perfectly. For
now, I am running on batteries for testing per this pic:

![board setup]({{ site.url }}/images/DSC_0277.jpg)
