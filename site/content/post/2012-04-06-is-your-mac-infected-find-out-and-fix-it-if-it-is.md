---
id: 4013
title: Is your Mac infected? Find out (and fix it if it is)!
date: 2012-04-06T17:05:06+00:00
author: Jorge Cortell
layout: post
guid: http://cortell.net/blog/?p=4013
permalink: /blog/2012/04/06/is-your-mac-infected-find-out-and-fix-it-if-it-is/
wpsd_autopost:
  - "1"
categories:
  - Geek Fun
  - General
  - Hacking
  - News
  - Technology
---
<a title="http://arstechnica.com/apple/news/2012/04/flashback-trojan-reportedly-controls-half-a-million-macs-and-counting.ars" href="http://arstechnica.com/apple/news/2012/04/flashback-trojan-reportedly-controls-half-a-million-macs-and-counting.ars" target="_blank">Over 600,000 Macs are infected with the FlashBack Trojan</a>. Is yours one of those? Let`s find out.

Open the Terminal (c`mon, be a hacker, not a slacker) and type:

<pre>defaults read /Applications/Safari.app/Contents/Info LSEnvironment</pre>

if it says:

> `The domain/default pair of (/Applications/Safari.app/Contents/Info, LSEnvironment) does not exist`

that means your Mac is ok so far (otherwise, go <a title="https://www.f-secure.com/v-descs/trojan-downloader_osx_flashback_i.shtml" href="https://www.f-secure.com/v-descs/trojan-downloader_osx_flashback_i.shtml" target="_blank">here</a>). 

Then type:

<pre>defaults read ~/.MacOSX/environment DYLD_INSERT_LIBRARIES</pre>

if it says:

> `The domain/default pair of (/Users/[your user name here]/.MacOSX/environment, DYLD_INSERT_LIBRARIES) does not exist`

that means your Mac is not infected (otherwise, go <a title="https://www.f-secure.com/v-descs/trojan-downloader_osx_flashback_i.shtml" href="https://www.f-secure.com/v-descs/trojan-downloader_osx_flashback_i.shtml" target="_blank">here</a>). 

Source FSecure via Ars <a title="http://arstechnica.com/apple/news/2012/04/flashback-trojan-reportedly-controls-half-a-million-macs-and-counting.ars" href="http://arstechnica.com/apple/news/2012/04/flashback-trojan-reportedly-controls-half-a-million-macs-and-counting.ars" target="_blank">Technica</a>.