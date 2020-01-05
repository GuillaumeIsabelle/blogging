---
ID: 1435
post_title: Particle fluid tips
author: gicomadmin
post_excerpt: ""
layout: post
permalink: >
  http://guillaumeisabelle.com/blogging/2020/01/04/particle-fluid-tips/
published: true
post_date: 2020-01-04 19:44:49
---
> Particle fluid tips If a collision/container wall is too thin, the particles can collide with the wall but the pressure solve step may not see it, causing particles to "stack up" against the wall instead of bouncing off it, making the liquid appear to compress and disappear. Increasing the thickness of the collision geometry will fix this (note that you can use different geometry for creating the collision field and for rendering, so you can still render a thin container wall). Source: *[Particle fluid tips][1]*

 [1]: https://www.sidefx.com/docs/houdini/fluid/tips.html