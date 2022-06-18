---
layout: post
title: Documentation - My Notepad
date: 2022-6-15 21:57:00 -500
categories: [homelab,documentation]
tags: [github,Jekyll]
pin: true
---

# Random Notes - My Notepad

I\'m completely new to most of the things i\'m working on in my homelab.  This is just my virtual notepad.  Its strickly for me to keep snippets of information to reference.  
\----

Launch Jekyll Locally
```bash
bundle exec jekyll s
```
<br>

Push New Content to github
```bash
git status
git add [. (for all), filename (for files)].
git commit -m "Description of Changes"
git push
```
<br>

Building your site in production mode
```bash
JEKYLL_ENV=production bundle exec jekyll b
```
<br>

