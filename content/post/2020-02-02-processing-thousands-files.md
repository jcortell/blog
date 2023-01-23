---
author: ""
date: "2020-02-02T01:00:24+02:00"
draft: false
title: "Processing thousands of files using Terminal commands"
tags: ["technology", "work", "geek"]
images: "https://p1.pxfuel.com/preview/595/744/913/monitor-screen-browser-computer.jpg"
comments: false     # set false to hide Disqus comments
share: true        # set false to share buttons
thumbnailImagePosition: left
thumbnailImage: https://p1.pxfuel.com/preview/595/744/913/monitor-screen-browser-computer.jpg
coverImage: https://p1.pxfuel.com/preview/595/744/913/monitor-screen-browser-computer.jpg
metaAlignment: center
coverMeta: out
---

How to fix a problem that spawns over more than two thousand files without spending days with a word processor? CLI to the rescue.

<!--more-->

Having a JAM[^jam] stack with a static generator CMS[^cms]  under VC[^vc] in Git with automated CI/CD[^cid] through a global CDN[^cdn] is great for many reasons (speed, security, scalability...) but what happens when a new version decides to change which characters are accepted in the build and which ones are deemed invalid? Then you have a problem that in my case spawn over more than two thousand files.

I'm not nearly as much of a CLI[^cli] master as my friends Alvaro or Santiago. But I love to learn new tricks, and get a kick out of the power of the terminal.

In this case I had to locate a number of "offending characters" (left overs from a previous blog engine migration, that handled the text encoding differently) in thousands of files, and then do a "replace with" in all of them at once.

What did I do? Thanks to tutorials by CLI Magic, Winaero, Linuxize, and Maketecheasier, I put together the following.

First, identify which files were causing trouble. After all, if it was just one or two, I could fix it manually. So I run (in the directory containing all my blog posts):

```
grep -iRl "&#"
```

Here are the options:
-i - ignore text case
-R - recursively search files in subdirectories
-l - show file names instead of file contents portions

The reason why I used "&#" is because of the offending text encoding always included that partial string.

Once I realized we were talking about over two thousand files, I decided to use the CLI in order to substitute the offending strings. I won't list them all, so I don't give away clues and vulnerabilities, but the general command I used is:

```
find . -type f -exec sed -i 's/&#8230;/.../g' {} +
```

And, just like magic, in the blink of an eye, all the offending occurrences of `&#8230;` were turned into `...`.

That is, in essence, what lies at the heart of modern software and data transformation. Unix, still so brilliant after over half a century.

[^jam]: JavaScript, APIs, and Markup
[^cms]: Content Management System
[^vc]: Version Control
[^cid]: Continuous Integration / Continuous Delivery
[^cdn]: Content Delivery Network
[^cli]: Command Line Interface
