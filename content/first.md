---
title: "First"
date: 2019-08-20T14:47:35+09:00
draft: false
images: ["images/ONE.jpg"]
featured_image: "images/ONE.jpg"
---
Hugo 0.57.0 had some well-intended breaking changes. And while they made a lot of sense, one of them made a little too much noise.

This release reverts the behavior for .Pages on the home page to how it behaved in 0.56, but adds a WARNING telling you what to do to prepare for Hugo 0.58.

In short, .Page home will from 0.58 only return its immediate children (sections and regular pages).

In this release it returns .Site.RegularPages. So to prepare for Hugo 0.58 you can either use .Site.RegularPages in your home template, or if you have a general list.html or RSS template, you can do something like this:


{{< figure src="/images/belluga.jpg" title="MOL ACE" >}}
