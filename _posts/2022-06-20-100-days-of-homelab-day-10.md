---
layout: post
title: 100 Days of Homelab [Day10]
date: 2022-6-20 19:20:00 -500
categories: [homelab,hardware]
tags: [Dell, r210ii, r220, OPNSense, Pi-Hole, heatwave,hyperionmedia.us,100DaysofHomeLab]
---

# DAY 10

Well, Sunday was horrible.  Air conditioner went out.  North Dakoka like most of the US was under a heat warning.  Hit 101F today outside AND in my apartment.  Needless to say, theRack was powered down.  Called my leasing company, schedule a replacement and then I crashed on my neighbors couch all day and slept while he was at work. Maintanence guy said he\'d replaced 14 units since Saturday.  Came up at 3pm and it was nice and cool.  Waited a few hours just enjoying the cool air before powering the rack back on

**NOTE** *You should always have your OPNSense and Pi-Hole vm\'s set to Auto-Start.*

So, managed to the theRack back up and running.  After the misreable day yesterday/last night, I decided to just chalk today up to a breather.

* **[COMPLETE]** Adjustest VM's for OPNSense and Pi-Hole to Auto-Start on Proxmox Boot.  Should resolve any future issues relating to restarting/cycle power etc and not having connectivity.
* **[INPROGRESS]** Replace Dell r210ii with Dell r220.  Was delivered today, and 32gb ECC 1600 Ram is due in Friday.

## Potential Day 11 Timeline
* Fix the template issues causing the /vault/index.html file so its correct and not blanks.
* Build my new desk from the 6\' Butcher Block Counter Top I recently purchased
* Update all firmware on the newly delivered Dell r220 in preerations for migrating r210ii Proxmox install with OPNSense and Pi-Hole to it.