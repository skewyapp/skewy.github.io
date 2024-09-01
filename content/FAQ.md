---
title: 'FAQ'
date: 2024-03-24T12:04:15+01:00
draft: false
menu:
  main:
    name: "FAQ"
    weight: 2
---

*Why do you not just use a 'block the microphone setting'?*

Can we be sure this actually works? Software settings can be overwritten by the operating system.

*Can Skewy decipher ultrasonic signals (i.e. 'who sent the signal?')?* 

To decipher a signal, the full signal would have to be recorded. In this case, the signal would have entered the device and would be read by the target, making the jamming obsolete.

*Is every detection a signal?*

No. For example, electronic equipment such as marten repellents for cars or induction cooktops can emit in the evaluated range of 17.8 to 20 kHz.

*Why 17.8 to 20 kHz?*

This range is based on technical literature for the ultrasonic signals in question. Most microphones and loudspeakers are developed for the audible range of 20 Hz to 20 kHz. Human hearing performance is low in the higher range, leaving 18 kHz to 20 kHz in the possible range while remaining inaudible. See Arp et al. (2016): Bat in the Mobile: A Study on Ultrasonic Device Tracking, chapter 3.1.

*Can I test the ultrasonic detection?*

Yes, an online tone generator can be used (for example, https://onlinetonegenerator.com/). More dedicated tests can be done with files from https://github.com/MAVProxyUser/SilverPushUnmasked.

*How often is an ultrasonic jamming signal emitted?*

Once per alarm. It is not emitted when the alarm timer is counting down. The shortest possible interval is 15 seconds. The jamming signal lasts approximately 8 seconds.

*Which processing algorithm is used?*

The Goertzel algorithm. It was chosen over a Fast Fourier Transform (FFT) because it is more lightweight, minimizing the drain on resources (battery and processing). Skewy focuses on whether an ultrasonic frequency is present, not the exact nature of it (see the second question, "who sent the signal?").

References:

Arp et al. 2017: Privacy Threats through Ultrasonic side Channels on Mobile Devices, TU Braunschweig. (https://www.sec.tu-bs.de/pubs/2017a-eurosp.pdf)

https://en.wikipedia.org/wiki/SilverPush 

https://techcrunch.com/2014/07/24/silverpush-audio-beacons/

https://www.comparitech.com/blog/information-security/block-ultrasonic-tracking-apps/ 

https://github.com/MAVProxyUser/SilverPushUnmasked 

https://arstechnica.com/tech-policy/2015/11/beware-of-ads-that-use-inaudible-sound-to-link-your-phone-tv-tablet-and-pc/ 


