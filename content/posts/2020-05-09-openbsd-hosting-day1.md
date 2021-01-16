---
layout: post
title: "OpenBSD Web Hosting: Day 1"
tags: 
- bsd
- webhosting
date: "2020-05-09"
description: "OpenBSD has its own webserver."
---

I've recently moved my host from my employer's shared hosting platform to a self-hosted OpenBSD server on my preferred cloud host. I've been wanting to play with the built-in [httpd(8)](https://man.openbsd.org/httpd.8) ever since I saw that it existed. The configuration itself is super simple, almost like my experience with Ruby's Sinatra framework. Apparently, in addition to LibreSSL, OpenBSD has it's own built-in Let's Encrypt client - [acme-client(1)](https://man.openbsd.org/acme-client.1). The configuration for this is also super simple. Just configure your ACME server, then your domain, the ASNs, the paths for your certificates, and then which server to sign. It follows the same config as [httpd.conf(5)](https://man.openbsd.org/httpd.conf), which is mentioned above.

This whole blend works nicely with this site, which is written with Jekyll, a static site generator developed in Ruby.

I don't understand why, but simple sometimes is better.
