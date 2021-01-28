+++
title = "OpenBSD Upgrade"
date = "2021-01-27T21:53:49-06:00"
author = ""
authorTwitter = "" #do not include @
cover = ""
tags = ["sysadmin", "openbsd", "bsd"]
keywords = ["openbsd", "openbsd 6.8", "sysupgrade"]
description = "A little bit late..."
showFullContent = false
+++

A little bit late, but we're up to date. Luckily, this goes for all sites, as there's no real CMS to break into. The upgrade was pretty easy - one simple command - sysupgrade. It downloaded all the filesets and the new kernel before unpacking and rebooting.

Also, there's a recent video about the recent sudo vulnerabilities. The recommendation was to move to doas and I couldn't agree much more. The config is stupidly simple - just look up "man 5 doas.conf". It's not as heady as a sudoers file at all. It's simple, to the point, and is constantly updated by the OpenBSD team the moment there is a security vulnerability. You can get it on almost any Linux or BSD. The Linux folk can use duncaen/OpenDoas from Github or off of the Arch AUR or repos.
