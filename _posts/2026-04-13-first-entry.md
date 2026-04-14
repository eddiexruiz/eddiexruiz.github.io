---
title: "First entry: Hi"
date: 2026-04-13
---

Ever since I had a computer I've have been trying to find my next project; wether setting up audio devies for music productions or spinning a small Maplestory server for me and my counsin; I have been flirting with various skills and technologies for a long time. As an adult as I progressively like to complicate my life with newer more complex proyects, I found myself not documenting my journey.

This leads me to start a project, pick up skills, learn through trial and move on with the next project. Though this issue also leads me to forget all my learning moments and stumble with previously encounter errors or issues and find myself with a new list of issues all because I have little to know documentation.

You can expect a wide range of subjects to be looked at as I go through my blogging journey. Starting with current passion project.

*-Setting up my HomeLab Server.-*

I have been working on lifting my server since last December and got a few cool components, including an ER605 Router which is a great all around router for anybody starting a home server. 

I have previously worked with setting up a Wireguard VPN with a raspberrypi and that worked a good 70% of the time. I didnt know why it didnt work or why it did work. 

Fast foward with my ER605 and I managed to set up My Wireguard working within ER605; It worked 95% of the time; that other 5% of the time was if I ever looked at the router the wrong way and tried to make it a bit more efficient. 

If I updated the a Client entry or the server it just wouldnt work. This had me recoverying a Backup configuration which magically had it working. 

I spent many early morning and late evenings trying to get this to work reliably. And that when I finally learned about CGNAT.

CGNAT is good networking solution for those uninitiated in the tech world; but for powerusers that want to get the most of their internet, it makes network routing a nightmare.

And after 4 months of accepting that my VPN had a 5% failure rate. The worse happened.

That 5% failure rate went up to 100%. I tried everything to get the VPN working again:

- Bouncing all my systems
- Reconfiguring the VPN Service
- Factory reseting my Router
- Trying a different VPN Service
- IPV6 routing (not supported by ISP)

I had given over a workweek's worth of troubleshooting to this issue and finally found a solution... contacting my ISP.

After explaining my issue and confirming with my ISP that I was behind a CGNAT and it was causing issues; they gladly removed me out of it.

One DDNS configuration later; and that 100% faliure transformed to a 100% success. 

Multi system reboots are not phasing my set up now.

There are other solutions that could handle this with ease and my resonds I left them as last resorts.
- A public Static IP (Additional costs)
- a VPS service (Addittional Costs + introducting an external system that needs)
- IPV6 if ISP supports it (not supported by ISP)

Now that I have a stable VPN connection; I know my work can progress at a constant pace.



