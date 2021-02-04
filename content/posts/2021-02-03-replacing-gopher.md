+++
title = "Replacing Gopher"
date = "2021-02-03T21:16:39-06:00"
author = "Josh Cain"
authorTwitter = "kmartkart" #do not include @
cover = ""
tags = ["software", "gemini"]
keywords = ["gemini", "gopher"]
description = "So... I found out something about Ubuntu..."
showFullContent = false
+++

The description is a bit clickbaity, innit? Well, apparently, if you go too long without updating Ubuntu, you won't be able to update Ubuntu. The server I had hosting my znc and gopher servers - agopherhole.tk - were running on Ubuntu 19.10. Well, it's 2021 now, and all the links to the repos in the APT configuration just weren't hitting any more. After trying a `do-release-upgrade`, I was prompted to upgrade any and all packages that needed an upgrade. But APT just couldn't pull those down. I had no access to the server, so I couldn't copy out important configuration, reinstall on the LTS, and try again. So, I copied out all the important configuration, dropped the server, and spun up a new one, with FreeBSD. However, after trying to get Gopher set up on that, it proved that it couldn't be helped.

Now I watch [distrotube](https://www.distrotube.com/), and he had a good video on the Gemini Protocol. It looks to be a modern version of Gopher, running off port 1965 rather than port 70. And the text/gemini syntax is more like Markdown than anything. So, taking a leap of faith, I moved from Gopher to Gemini. You can access the site from a Gemini browser at [gemini://agopherhole.tk](gemini://agopherhole.tk).
