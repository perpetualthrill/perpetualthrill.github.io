---
title: Successful isolation with Silicon Labs Si8621 digital isolator
---
Ok, now we are in business. Here is the current prototype, with the [Olimex
MOD-EKG](https://www.olimex.com/Products/Modules/Biofeedback/MOD-EKG/) under battery power on one side of the isolator
and the microcontroller and computer on the other.

![successful isolation proto]({{ site.url }}/images/DSC_0501-2.JPG)

Aaaand, here's the output from that run through a processing sketch that shows a totally reasonable ECG. Success!

![raw output processing sketch]({{ site.url }}/images/DSC_0500-2.JPG)

Lastly, here is that same output, captured to a CSV and high-pass filtered with a 21 sample mean. Even with heavy filtering,
the QRS complex is super clear and easy to spot. Excellent.

![filtered data graph]({{ site.url }}/images/heartrate-21-sample.jpg)

