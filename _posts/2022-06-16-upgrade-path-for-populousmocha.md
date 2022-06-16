---
title: Upgrades - Upgrade Path for a Fellow Discord Member
date: 2022-6-16 14:10:00 -500
categories: [homelab,hardware]
tags: [Dell,Intel,Samsung EVO,DVD SwapKit,SK Hynix,h200e,EMC,HGST,upgrades]
---

# Potential Upgrades for populousmocha

Talking with populousmocha on Discord and he\'s using some outdated gear.  Told him I would research him an upgrade path that would meet his budget, give him more efficient power and expandability down the road.  So below you will see what I\'ve suggested for him

He initially stated a budget of around $700, but I think we can smoke that and get it way down and save his pocket book.  

## Hardware
* $250.00 Dell [PowerEdge r720 with (2) E5649 CPU\'s and 128gb RAM](https://www.ebay.com/itm/115378774222)
    - $80.00 [(2) Intel Xeon E5-2690 V2 3.0GHz 10 Core LGA 2011](https://www.reddit.com/r/homelabsales/comments/uniaxf/fs_usnh_on_sale_intel_xeon_e52690_v2_30ghz_10/) *cpu upgrade*
    - $40.00 [(2) Samsung EVO 128gb SSD\'s in ZFS Mirror for Boot](https://www.ebay.com/itm/394107763341) *zfs mirror OS boot drives*
    - $7.00 [(1) DVD Swap Kit for SlimLine DVD](https://www.ebay.com/itm/313349100635) *for utilizing the dual boot ssd\'s above*
    - $40.00 [(4) Lot of (2) 2.5\" Dell r720 HDD Caddy](https://www.ebay.com/itm/175279047981) *could start with (2) sets of 2 just for his 2tb hdd\'s he already has*
    - $75.00 (1) Up to 4 [SK Hynix GoldS31 1tb SSD](https://www.reddit/com/homelabsales/) *for VM Storage* **Optional Later Upgrades**
    - $40.00 [(1) Dell h200e HBA flashed in IT Mode](https://www.ebay.com/itm/144410379778) *for connecting the DAS/JBOD* **Optional Later Upgrades**
* $225.00 [EMC KTN-STL3 3.5\" 15-Bay SAS2 JBOD](https://www.ebay.com/itm/154980724535) **Optional Later Upgrades**
    - $240.00 [(15) HGST 3tb SAS HDD\'s](https://www.reddit/com/homelabsales/) **Optional Later Upgrades**

### Price Break Down

Essentials: +/- $397 Server + CPU\'s + Boot SSD\'s + DVD SwapKit + 4 2.5\" Caddys<br>
Optional Server Upgrades: +/- $320 for VM Storage SSD\'s in a raidz1 and 4 more 2.5\" Caddys<br>
Optional Storage Upgrades: +/- $550 for 45tb Storage<br>

### My Thoughts

The idea behind this is the utilize the readily available r720 sff chassis\'s that are scattered everywhere on ebay for the sdd 2.5 bays to carry the SSD\'s for VM/Higher Speed Storage and then down the road add on an External HBA flashed in IT Mode to add to the FileServer VM and have the ability to start adding 3.5\" hdd\'s

The vm storage ssd and hdd models chosen would of course be whatever the best price per tb at the time is.

Hopefully this helps populousmocha or anyone who is looking for a potential upgrade.