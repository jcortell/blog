---
id: 5049
title: Testing a simple hack
date: 2014-01-04T14:51:25+00:00
author: Jorge Cortell
layout: post
guid: http://cortell.net/blog/?p=5049
permalink: /blog/2014/01/04/testing-a-simple-hack/
categories:
  - Geek Fun
  - General
  - Hacking
  - Personal
  - Technology
---
I use _qtranslate_ as a multi-language plugin for my blog. It&#8217;s an excellent solution, but the problem is that everytime Word Press is updated, it takes days, and sometimes weeeks, for the plugin author to update it.

So, tired of waiting, I have found a quick and simple hack to make it work with the latests WP 3.8 update: edit qtranslate.php to

> define(&#8216;QT\_SUPPORTED\_WP_VERSION&#8217;, &#8216;3.8&#8217;);

You&#8217;re welcome 😉