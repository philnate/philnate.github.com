---
layout: post
title: "Restoring Windows"
date: 2007-12-05 23:07
comments: true
categories: ["others"]
tags: ["bootloader", "recovery", "windows"]
---
Just the latest example how stupid I can be sometimes:  
I've dropped yesterday my Linux Partition from my laptop. It wouldn't be that problematic if it hadn't the Boot session on it. Anyway I didn't noticed that big mistake until I restarted my Laptop and encounter some Error while Loading GRUB.  
After the first seconds of thinking, what happened, I started to knock my head against the table(not really:)). As soon as I stopped to hate myself I made a search for a solution and quickly found an Answer: [Start your PC with your Recovery CD](http://www.pcwelt.de/forum/windows-xp-server-2003/158389-grub-bootloader-gel-scht-xp-startet-2.html) and run fixmbr and fixboot. Ok, no big deal...as long as you have your Recovery CD with you, but I didn't...(second time some knocking, was hearable).  
So my next try was to get some Recovery Application on the base of some small DOS Boot, I found quickly something, anyway it didn't worked for XP(at least for my PC it didn't).  
Next I've inserted the Vista Recovery from some friend( I would like to mention that without any Install you can run already some Safe-Mode like Vista...with working Notepad, aso.). I was even able to start a Cmd.exe, but the next shock wasn't far as I noticed that **fixmbr**&amp;**fixboot** didn't worked within Vista. A new search was on the way, on how to get fixmbr&amp;fixboot working on Vista Recovery CDs, again I had luck and found soon, [a solution](http://www.linuxforums.org/forum/installation/94066-need-fix-mbr.html)...you have to call them as Parameter through some other application:  
<code>  
bootrec.exe /fixmbr  
bootrec.exe /fixboot  
</code>  
I've applied both commands, the had be done correctly and after a Restart I was able to Boot Windows again. The only good point is that I don't have to take care on startup if the correct OS is selected, anymore :).  
A side note for the next time I make any changes to an OS, be sure to have the recovery CD near myself!
