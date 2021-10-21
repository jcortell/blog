---
author: ""
date: "2021-10-21T04:00:24+02:00"
draft: false
title: "Testing Two-Up in Hugo"
tags: ["personal", "technology"]
images: "https://c0.wallpaperflare.com/preview/524/860/912/screen-code-coding-programming.jpg"
comments: false     # set false to hide Disqus comments
share: true        # set false to share buttons
thumbnailImagePosition: left
thumbnailImage: https://c0.wallpaperflare.com/preview/524/860/912/screen-code-coding-programming.jpg
coverImage: https://c0.wallpaperflare.com/preview/524/860/912/screen-code-coding-programming.jpg
metaAlignment: center
coverMeta: out
---

GoogleChromeLabs has released an interesting component to compare two DOM elements: [two-up](https://github.com/GoogleChromeLabs/two-up). Let's try it.

<!--more-->

First, let's make sure [Hugo](https://gohugo.io) (the static generator I use in this blog) renders the HTML inline correctly, which you can accomplish adding a [shortcode template](https://gohugo.io/templates/shortcode-templates/) to insert raw HTML into the post's markdown (thanks for the idea, [Ana Ulin](https://anaulin.org/blog/hugo-raw-html-shortcode/)) simply adding a shortcode template called `rawhtml.html` in `layouts/shortcodes/rawhtml.html` in your Hugo installation. So, create an HTML document with that name, in that directory, with this content:

`<!-- raw html -->
{{.Inner}}
`

Now all you need to do is to write your HTML code inside the Hugo markdown using this shortcode:

`{{< rawhtml >}}
    Pon aquí tu HTML
{{< /rawhtml >}}
`

And to try Two-up, what's the HTML code you have to use (calling the JS externally)? Easy!

`<script src="https://unpkg.com/two-up-element@1"></script>

<two-up>
  <div><img src="https://lh3.googleusercontent.com/t-t_jepUsuxueR9K1FIYOybuiefOriG6fCrxBJSHWs56dPvztmrcknPmkemzQSlr38T9HJC6LwOfaVD0yLmpaB0ydCLHqwv8jfaJ9V50OWNORczRJjgD5uoAt1VQZ1BWLX3ueEq3NeU=w1920-h1080" alt="before"></div>
  <div><img src="https://lh3.googleusercontent.com/DBgFrRegPOAmVbaDj_ecDZdn5nJ5B_YeTtj3YtO2gMMgPC5hIqk2m-fVfjWOPj7hG0-C7A6FxQcqILUSR0hM98uKuxwWJHA6mVGZEsgwqzeqLowftjeUnfNp10xS6bzQ7IDUoDl6Mq4=w1920-h1080" alt="after"></div>
  `

Sorry for the pictures but it's the first ones I found in my collection. Now imagine all the uses you can give this (compare compression levels, modifications, versions...):

{{< rawhtml >}}

<script src="https://unpkg.com/two-up-element@1"></script>

<two-up>
  <div><img src="https://lh3.googleusercontent.com/t-t_jepUsuxueR9K1FIYOybuiefOriG6fCrxBJSHWs56dPvztmrcknPmkemzQSlr38T9HJC6LwOfaVD0yLmpaB0ydCLHqwv8jfaJ9V50OWNORczRJjgD5uoAt1VQZ1BWLX3ueEq3NeU=w1920-h1080" alt="before"></div>
  <div><img src="https://lh3.googleusercontent.com/DBgFrRegPOAmVbaDj_ecDZdn5nJ5B_YeTtj3YtO2gMMgPC5hIqk2m-fVfjWOPj7hG0-C7A6FxQcqILUSR0hM98uKuxwWJHA6mVGZEsgwqzeqLowftjeUnfNp10xS6bzQ7IDUoDl6Mq4=w1920-h1080" alt="after"></div>
</two-up>

{{< /rawhtml >}}
