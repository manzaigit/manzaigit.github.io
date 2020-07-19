---
layout: post
title:  "Repurpose"
date:   2019-10-13 13:00:00 +0800
categories: tech
---

tl;dr: If your desktop / laptop breaks down, it doesn't always mean that everything is broken (it's usually because of 1 critical component). Out of all the components, one of the useful parts that can still be used (without going through too much trouble) is your **internal** hard disk. You can repurpose it with a few tweaks and get additional storage space!  

Caveats: Some laptops aren't easy to disassemble and will require [special screwdrivers](https://en.wikipedia.org/wiki/Torx) but most of them are easy. Money spent to buy these equipments < value you will unlock by reusing parts that still work. :) 
<br><br>

---
<br>

### Backstory

Recently, my all-in-one desktop had issues with starting up and I accidentally killed the hard disk by switching off the power while it was booting up... it just crashes everytime it tries to start (I'm guessing the disk got scratched and some parts that were essential for the booting process got corrupted - a few of my files were corrupted too) but luckily I could still access the command prompt in the Windows Recovery Environment. But [transferring files from a hard disk to another via the command prompt (with the xcopy command) was a huge pain](https://support.microsoft.com/en-us/help/323007/how-to-copy-a-folder-to-another-folder-and-retain-its-permissions) especialy when my hard disk was bigger than my external HDD, had to transfer things to and fro another laptop multiple times.

So I got a [new SSD (an affordable Samsung EVO860 500GB)](https://www.courts.com.sg/samsung-mz-76e500bw-2-5in-860-evo-500gb-ssd-internal-ssd-ip137598) and got it set up pretty quickly and the desktop revived. Guess the hypothesis was quite correct. 

### Main content

I have a habit of disassembling my old/spoilt computers and sending everything except the hard disk for recycling. So this incident made me realise that they could be repurposed as an external HDD - but it was more trouble than I expected. I did quite a lot of due dilligence, but still ended up buying the wrong things. But with the following information gathered from this experience, repurposing is actually as simple as:

1. Disassembling your computer
2. Getting the correct SATA-USB cable 
3. Plugging it into another computer just like what you do with a portable HDD

### Essential background knowledge

1. IDE/PATA vs SATA

    I had a range of hard disks (made in 2006, ~2012, 2016) and the 2006 was an 80GB one (from an ancient NEC laptop!)

    Here's how to [differentiate between them](https://www.reclaime.com/library/how-to-tell-ide-from-sata.aspx), basically SATA has a flatter connector while IDE has 2 rows of wire ends. The latter is much older (it's the 2006 one for mine!)

    There's 2 types of SATA: 2.5 inch and 3.5 inch, the latter is generally older than the former (and mine was both 2.5 inch HDDs).

2. Enclosure or Cable? 

    Many websites recommended [buying an enclosure](https://www.howtogeek.com/268249/how-to-turn-an-old-hard-drive-into-an-external-drive/) but I wasn't a fan of that idea. Instead, I bought the [cheapest (but still legitimate looking) SATA to USB cable I've found](https://www.qoo10.sg/item/USB-3-0-TO-2-5-INCH-SATA-CABLE-CONVERTER-ADAPTER-HARD-DISK-6/603602163?banner_no=1305330) and it does light up but the hard disk doesn't get recognised by the computer (and the hard disk isn't spinning at all). Naturally, all the debugging didn't work. 

    On hindsight, I should've spent a few more dollars to get one with [extra power supply](https://superuser.com/questions/1372617/can-a-sata-to-usb-cable-run-a-sata-hard-disk-off-a-usb-port). Got one from [here](https://www.lazada.sg/products/free-uk-power-adapterugreen-sata-to-usb-adapter-usb-30-20-cable-to-sata-converter-for-samsung-seagate-wd-25-35-hdd-ssd-hard-disk-usb-sata-adapter-uk-plug-intl-i6393383-s8040426.html) and it generally worked well. So you don't really need an enclosure after all (if you're okay with leaving the hard disk in the open - just remember to keep it in an airy place, wipe it when it's dusty, or just use it only when you need to).
