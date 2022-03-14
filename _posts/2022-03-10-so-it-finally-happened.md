---
title: "So, it finally happened!"
excerpt_separator: "<!--more-->"
categories:
  - Blog post
  - Personal
tags:
  - Blog post
  - Personal diary
  - jekyll
  - Github pages
author_profile: true  
---

## So, it finally happened! I'm starting my very first own blog!


I remember when I first decided to dedicate myself into learning coding back in 2017 after graduating with a BFA in Design at SVA -- I signed up for General Assembly intensive Full-Stack Development. 

Did I become a coder after that? yes, in my mind, but long story short, not really.

Although I did learned hack of a lot of new stuff there over the course of 12 weeks, it felt like I got every little pieces of the puzzle but I didn't get to put them together into one completed result.

With my eagerness to find ways to understand code better and my designer mind & eyes that naturally exist within myself, I found an MFA program in Design & Technology at Parsons School of Design where I thought the learning experience was above and beyond my expectations for sure.

Besides all of the cool stuffs I learned like building physical interactive prototypes with Arduino, creating amazing visuals digitally with Processing and P5.js, producing projection mapping on my personal objects and spaces, creating music with live code in Algorave class, and crafting computational circuits on physical materials, building single web pages with JavaScript seemed very realistic practices to me after all.

As I was just a beginner coder, knowing how to incorportae API and manipulate its JSON data with a few blocks of code was just enough for me to pat myself on the back, haha.

Ultimately, I was able to take a little step by step to create my own portfolio website and work through presenting my newbie projects on a single website, hosted on [Github Pages](https://pages.github.com/)!!

But today, I'm replacing my personal website with a whole new something I found out about recently - Jekyll, aka simple, blog aware, static site generator!

Jekyll is already being widely used among many other developers and there were definitely many resourceful documentations from them, however, it did take me a while to understand the whole concept of its templates, dynamic components, markdown usages, and customizing things to begin with.

After all the hectic moments figuring things out about [Minimal-Mistakes Jekyll theme](https://github.com/mmistakes/minimal-mistakes), I'm just writing my very first blog post with my excitement to have found a perfect way to express bits of my thoughts, keep records of my daily studies, and to collect all the things I want to remember - notes, advices, inspirations, and code examples and so on... Thanks to Michael Rose!

Jekyll makes it so much easier for me to create a page or post a blog to my website - Yay! I don't need to worry about creating separate HTML files now.

I might not be a good writer at all but I think starting today, using Jekyll as my personal journaling is going to be a great opportunity for me to express my journey on personal development and sharing any small knowledge or showing what I'm capable of. Maybe for the sake of better future me

{% capture fig_img %}
![previousPortfolio]({{ '/assets/posts/post1/previous-portfolio.jpg' | relative_url }})
{% endcapture %}

{% capture fig_gif %}
![gif]({{ '/assets/posts/post1/gif.gif' | relative_url }})
{% endcapture %}


<figure>
  {{ fig_img | markdownify | remove: "<p>" | remove: "</p>" }}
  {{ fig_gif | markdownify | remove: "<p>" | remove: "</p>" }}
  <figcaption>what my previous portfolio website looked like</figcaption>
</figure>








