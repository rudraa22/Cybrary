# Zero Trust Architecture (ZTA)

## What is it?
Zero Trust is a security model based on the principle: **"Never trust, always verify."**

Unlike old-school security that assumed everything inside the network is safe,
Zero Trust treats EVERY request — internal or external — as potentially hostile.

## Core Idea
Think of it like a nightclub with a bouncer at every door, not just the entrance.
Even if you're already inside, you still need to show ID at every room.

## Key Principles
- **Verify explicitly** — Always authenticate and authorize using all available data
- **Least privilege access** — Give users only the minimum access they need
- **Assume breach** — Design as if attackers are already inside

## Real-world use
- Remote workers accessing company systems → verified every time
- IoT devices on a network → isolated and monitored
- Cloud environments → no implicit trust between services

## Why it matters now
Nation-state attacks (like Volt Typhoon by China) exploited trusted internal devices.
ZTA limits the damage even when attackers get in.

## Tools involved
- Multi-Factor Authentication (MFA)
- Identity and Access Management (IAM)
- Micro-segmentation
- Endpoint Detection & Response (EDR)

## Status: Learned ✅
Date: 2026-06-24
