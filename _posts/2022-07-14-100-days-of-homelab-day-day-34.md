---
layout: post
title: 100 Days of Homelab [Day34]
date: 2022-7-14 21:00:00 -500
categories: [homelab,hardware]
tags: [Dell,iDRAC,TrueNAS,Samsung,r220,100DaysofHomeLab]
---

# DAY 34

Woke up exited as I got a notice that I had a package on the way.  Yup, that\'s correct, the iDRAC module was on the way.  Waiting patiently, by refreshing the delivery screen every 5 minutes, I surfed youtube and decided I would power down my TrueNAS VM and pull all my SSD\'s to run health checks on them and add labels with the date/health% on them for "bookkeeping".

DONE, iDRAC Module is in, didn\'t come with an Enterprise License so I had to install the 30 Day Trial while I figure out what to do about this.  I don\'t really want to pay 50 bucks to some random ebay seller with a key-gen program.

Bad News came shortly after ATTEMPTING to power on the r220.  Stuck at Configuring Memory...  This isn\'t good.  After spending an hour swapping every configuration possible, reading documentation on the r220 and some google work.  The Results, yup, ordered the incorrect ram.  APARTENTLY the Dell r220\'s use Unregistered Ram. SO the (4) 8gb of 12800r RAM I just purchased will not work.  Looking for (4) 8gb of 12800e now.  Seems to be a unicorn, so this is cost a bit.  Friday I\'m going to pull the 16gb from my r210ii and see what it is and possible put the ram that the r220 came with in the r210ii and use the 16gb in the r220 until I can locate 32gb of Unregistered.

With the r220 sporting the RAM it came with when purchased the new few hours were spent getting the BIOS on the r220 configured and upgrading all of the firmware.

Next was to plug a 256gb SSD and all my Samsung EVO 500gb SSDs.  Install Windows and run Samsung\'s SSD Utility and get health reports on all the SSD\'s.  Decided to slap a piece of tape on each with the date and its Health Percentage.  These SSD\'s will run pretty long as they run the Raid0 array i use for my torrents.  Once the *Linux* ISO\'s are on the array they just sit there so the SSD\'s do not see much writing, just the random reads here and there.  The array did consist of (3) 512gb SSD\'s but I have a 4th I\'m adding, so I will need to move all the files off, delete the vdev in TrueNAS and rebuild it with the 4th SSD in it.  I'll do that this weekend.

Listed the [(4) Samsung 8GB 2Rx4 PC3L-12800R DDR3](https://www.ebay.com/itm/144646243295) on ebay.  Hopefully I can recover some of the cost before finding the 12800r I need.  Feel free to take a peak and send an offer if you need any ram.

Tomorrow my monitors are due in and we can get the Tripple-Monitor Setup done. Until then...

* **[COMPLETE]** Install iDRAC Module into r220
* **[INPROGRESS]** REODER 32gb of 12800e RAM for r220
* **[COMPLETE]** Test all my SSD's in my r720 and get health reports on them all
* **[INPROGRESS]** Add in 4th 500gb Samsung EVO SSD to the Torrent Array
* **[INPROGRESS]** Pictures for Craigslist/Reddit Sales Threads

## Potential Day 35 Timeline
* Fix the template issues causing the /vault/index.html file so its correct and not blanks
* Replace Loud AF 80mm fans in the 4u Server with the new ones from Amazon
* Update all firmwares r220
* Pictures for Craigslist/Reddit Sales Threads
* Setup Triple-Monitor Desk mount with new monitors
