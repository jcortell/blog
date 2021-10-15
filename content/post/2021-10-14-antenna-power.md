---
author: ""
date: "2021-10-13T04:00:24+02:00"
draft: false
title: "Lowering my laptop's antenna power"
tags: ["personal", "technology"]
images: "https://res.cloudinary.com/jcortell/image/upload/v1634282494/Personal/blurredCLItxpower.png"
comments: false     # set false to hide Disqus comments
share: true        # set false to share buttons
thumbnailImagePosition: right
thumbnailImage: https://res.cloudinary.com/jcortell/image/upload/v1634282494/Personal/blurredCLItxpower.png
coverImage: https://res.cloudinary.com/jcortell/image/upload/v1634282494/Personal/blurredCLItxpower.png
metaAlignment: center
coverMeta: out
---

A USB-C multi-adapter kept misbehaving. It seemed to be interference from the laptop's antenna. So I decided to turn the antenna's power down. Here's a little how-to to save you the trouble of hours of a poorly documented process.

<!--more-->

Laptops are becoming lighter and more compact. Portability is a big plus, but there are also some drawbacks, like repairability, or the potential for interference.

My Dell DA200 USB-C multi-adapter never worked properly. If I connected everything (Ethernet cable, HDMI/VGA, and USB), at least two of those things would not work. For a long time I did not care, as I used it on the road and all I cared about was doing a presentation for a customer, or having an external mouse. But as I tried to use it from work, connected to the keyboard and external monitor, it bugged me. So I turned to the friendly online community to check possible causes of this malfunction.

That's when I learned about tuning your laptops' antenna power. In theory, the proximity of the adapter to the antenna is what was causing the malfunction.

> Fun fact: Dell's XPS laptops have USB-C connectors on both sides of the machine. Both can take the power adapter. But only one has an icon indicating power charge (⚡). Why? Paraphrasing a Dell engineer: 'if we didn't place any icon on either side, people would call tech support to find out how to charge the laptop... and if we placed it in both sides, it would create confusion and people would call tech support to find out which side was the right one, so we chose to place it on one arbitrary side'.

It turned out not to be the cause for my DA200 malfunction, and I ended up buying another adapter that allows me to have a triple monitor set up (sweet!). But I went into the antenna power rabbit hole. Here's the lowdown.

Long story short:
* Modifying your laptop's antenna power (within certain limits) has no effect on your wifi coverage.
* You shouldn't **increase** your laptop's antenna power, because you don't gain anything, and it could be against the law (each country regulates the power and frequencies of telecoms equipment).
* You **should lower** your laptop's antenna power, because you will save on power, which is good for the environment, your electricity bill, and for your laptop's battery.
* Manufacturers will not make that information easily available in most cases. And when they do, they assume you use a Microsoft Windows operating system and want you to mess with the BIOS.

So, how do you do it if you use a GNU/Linux system, like I do?

4 easy steps:

* Select the right interface (and name) by opening your CLI and typing `netstat -i`. In my case it was `wlp60s0`.
* Check the details, including power, by typing `iwconfig [interface name]`. In my case it was Tx-Power = 22 dBm.
* Reduce the power, by typing `sudo iwconfig [interface name] txpower [desired number]`. In my case I went down to Tx-Power = 11 dBm. Enter the password for `sudo`.
* Check that it worked by typing again (or using the arrow key to cycle through your recent commands) `iwconfig [interface name]` and checking the Tx-Power.
* The change is not permanent, so when you log out and back in, it will be back to the default. There are several ways to make it permanent, but I'll leave that for you to research, as that's very well documented online.
