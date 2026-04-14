---
title: "First Entry: Hi"
date: 2026-04-13
tags: [homelab, vpn, wireguard, networking] 
---

Ever since I had a computer, I’ve been chasing my next project.

From setting up audio devices for music production to spinning up a small MapleStory server for me and my cousins, I’ve always been exploring different technologies. Over time, that curiosity turned into a habit: start a project, learn a lot, and then move on.

The problem? I never documented anything.

That meant I kept running into the same issues over and over again, relearning lessons I had already figured out before.

So this blog is my attempt to fix that.

## Current Project: Home Lab Server

Right now, I’m focused on building out my home lab.

I started working on my server last December and picked up some solid components along the way, including the TP-Link ER605, a great entry-level router for anyone getting into home networking.

Before this, I had a WireGuard VPN running on a Raspberry Pi. It worked... about 70% of the time.

The problem was: I had no idea *why* it worked, or why it didn’t.

## The 95% Problem

After upgrading to the ER605, I set up WireGuard directly on the router.

This time, it worked 95% of the time.

The remaining 5%?

If I changed *anything* a client config, a setting, anything it would break. The only fix was restoring a backup that somehow “just worked.”

That’s when things got frustrating.

## When 5% Became 100%

Eventually, that 5% failure rate turned into a full 100% failure.

Nothing worked anymore.

I tried everything:
- Rebooting all systems  
- Reconfiguring WireGuard  
- Factory resetting the router  
- Switching VPN methods  
- Testing IPv6 (not supported by my ISP)

After spending way too many late nights troubleshooting, I finally confronted the real issue:

## CGNAT

I was behind CGNAT.

For most users, CGNAT is fine. But if you're trying to host services or run a VPN, it becomes a nightmare.

## The Fix

I contacted my ISP.

After explaining the issue, they confirmed I was behind CGNAT and removed me from it.

One DDNS setup later, and everything changed:

- 100% failure is now 100% success  
- Stable connections  
- No more random breakage  

## Alternatives I Considered

There were other options, but I left them as last resorts:

- Static public IP (extra cost)  
- VPS tunneling (more complexity + cost)  
- IPv6 (not supported by my ISP)  

## Where I’m At Now

Now that my VPN is stable, I can finally move forward with my lab without fighting my network every step of the way.

This time, documentation is part of the process. 
