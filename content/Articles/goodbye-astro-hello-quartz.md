---
title: Goodbye Astro, hello Quartz
tags:
  - software
  - web
---
I've been racking my head over the future of my site. The main reason for this is that I've moved to using [Obsidian](https://obsidian.md) to write my posts in and I really like it, but my past site was making heavy use of MDX which is essentially Markdown but you can add React components in. I kept having this strong feeling of, "I just want to fucking write, man" that my old Astro theme was unfulfilling. In fairness, the theme I was using ([astro-erudite](https://astro-erudite.vercel.app)) was very much geared as a nice-looking base for web developers to work on top of, and I am *not* a web developer in the slightest.

The reason for this was that I wanted to use Obsidian directly, and Obsidian doesn't really like using MDX. You can get Obsidian to load them via plugins, but you lose pretty much everything that requires Markdown processing and thus what makes Obsidian what it is, such as linked attachments and heading-based outlines. It just wasn't the right tool. Furthermore, Obsidian allows for embedded HTML but it knows pretty much nothing about the React components and thinks they're just generic HTML, which Obsidian will attempt to render.

I also tried Visual Studio Code directly, but the spell-check plugin I use does not support MDX. So close, yet so far. 🫠

I was nearly ready to go "fuck it" and spend some money on a WordPress or Ghost subscription, but then I realised what I wanted wasn't just an easy to use <abbr title="Content management system">CMS</abbr>, I wanted to write directly from Obsidian. I wanted Obsidian to **be** my CMS.

And this is where Quartz comes in. It's essentially a static site generator built on Eleventy, intended meant for "digital gardens" which a [dedicated subreddit](https://www.reddit.com/r/DigitalGardens/) describes as "personal wikis, digital spaces of notes & thoughts". To me, it's a bit like a personal diary that you're publishing to the internet. And it's got first-class support for Obsidian in one of the few templates available. I won't lie, I am still trying to get used to the "digital garden" mentality which heavily favours looseness, while I'm still stuck in the mentality that everything I write here *must* be a blog post (including this one!), but I think the looseness will be beneficial for me. I'm not worrying too much about themes or injecting JavaScript components into my site or coding a "collection". *I can just fucking write, man.*

There are some things I'd like to tweak - for example, the colour scheme was quickly adapted from my fursona's avatar.