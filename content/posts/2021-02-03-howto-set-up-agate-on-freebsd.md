+++
title = "How to set up Agate on FreeBSD"
date = "2021-02-03T23:09:03-06:00"
author = "Josh Cain"
authorTwitter = "kmartkart" #do not include @
cover = ""
tags = ["freebsd", "gemini"]
keywords = ["", ""]
description = "The simple instructions on how to set up a Gemini server on FreeBSD"
showFullContent = false
+++

It's sort of simple. You'll need a few things, really.
- Rust (Can be installed via rustup.rs)
- Certbot (`pkg install py37-certbot`)

## Setup
The first thing you are going to want to do is to install Rust and Certbot. Once those are installed, follow the instructions below. Replace <domainname> with your full domain name.

1. `cargo install agate`
2. `certbot certonly --standalone -d <domainname>`
3. `agate --content path/to/content/ --key /usr/local/etc/letsencrypt/live/domainname/privkey.pem --cert /usr/local/etc/letsencrypt/live/domainname/cert.pem --addr 0.0.0.0:1965 --hostname <domainname> --lang en-US`
4. Add a .gmi file to the content directory. 

A .gmi file is based off of Markdown with it's headers, bullets, and ordered lists. Links, however, are not inline. Rather, they are denoted by an `=>`. Links are easier than Gopher though. Take this example to the home page:

Gemini Link
`=> https://jdcain.me A blog`

Gopher Link
`hA blog<tab>URL:https://jdcain.me`

A bit clunky, I can assure you. The 'text/gemini' markup is simple and modern.