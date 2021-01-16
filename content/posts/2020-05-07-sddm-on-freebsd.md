---
layout: post
title: "SDDM on FreeBSD"
tags: 
- bsd 
- freebsd
- display manager]
date: "2020-05-07"
description: "Booting simpler."
---

So, I lied. I'm back on FreeBSD. Mainly because I couldn't live without my Spotifyd and spotify-tui. This time around, I put sddm as part of the startup process. It was simple. Just had to install from pkg. Once installed, I edited my /etc/rc.conf to include `sddm_enable="YES"`. 

After this was set, I went into /usr/local/etc/sddm.conf and set the theme: 

>`[Theme]`  
>`Current=sddm-freebsd-black-theme`

(Sidenote: This theme is also available in pkg)

I've got a nice welcome screen greeting me instead of the console. Though, the console is always sexy.
