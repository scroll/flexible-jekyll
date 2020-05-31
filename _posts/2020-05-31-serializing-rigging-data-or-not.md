---
layout: post
title: Should you serialize your rigging data or not?
date: 2020-05-31 13:32:20 +0300
description: Deciding if and when you should serialize your rigging data.
img: serialize.png # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [Rigging, Pipeline]
---

![]({{site.baseurl}}/assets/img/serialize.png)

This blog post is more about a rigging pipeline patterns rather than how to actually do rigging data serialization. For the latter, there are multiple articles on the subject and we are not going to discuss it here. 
So let's talk about one such rigging pipeline pattern. 

Before we dive in to explore it, let's talk about a few requirements first. Regardless of what type of studio you work at - VFX, Feature Animation or Games, it is almost certain that you probably have the requirement to rebuild your rigs. This is mostly a production requirement - if you want to stay competitive you don't want to lose time and build your rigs by hand from scratch all the time. Most probably you have some kind of framework or modular rigging system that does this for you. Rig requirements change constantly throughout the production so being able to push a button and rebuild a rig after the requirements changed is the most logical step. But being involved in multiple studios and pipelines during the years I have observed two patterns for doing that. One we will call "data serialization"
