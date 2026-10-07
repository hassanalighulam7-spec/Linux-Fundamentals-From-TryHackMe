# Offensive Security Intro

**Platform:** TryHackMe
**Path:** Pre Security → Introduction to Cyber Security
**Status:** ✅ Completed (100%)

## Overview

A short, beginner-friendly room where I attacked a fake banking website in a safe, legal lab environment. The goal was to experience what an ethical hacker does: find weaknesses the way an attacker would, so they can be fixed before real attackers use them.

## What is Offensive Security?

Offensive security means thinking and acting like an attacker to find vulnerabilities in a system. Ethical hackers do this **with permission**, and their findings help organizations improve their defences.

## Tasks Summary

| Task | Title | What I did |
|------|-------|------------|
| 1 | Think like a Hacker! | Learned the mindset and role of an ethical hacker |
| 2 | Starting the Lab | Launched the virtual lab and the target website |
| 3 | Find Hidden Pages | Used a discovery tool to find pages not linked on the website |
| 4 | Attack the Admin Page | Targeted the admin login page to gain access |

## Key Concepts

- **Hidden content discovery:** Websites often have pages that are not linked anywhere (admin panels, old pages, test pages). Attackers search for these by trying lists of common page names.
- **Weak authentication:** An admin login protected by a weak or guessable password can be attacked by trying many passwords automatically.
- **Impact:** Once an attacker reaches an admin page, they may be able to view or change sensitive data.

## Defensive Takeaways

Since my goal is a career in defensive security (SOC Analyst / Cloud Security), here is what this room means from the defender's side:

- Hidden pages are **not** secure just because they are not linked. Sensitive pages need proper access control.
- Admin panels should use **strong passwords, multi-factor authentication, and login attempt limits**.
- Repeated failed logins and large numbers of requests to non-existent pages show up in logs. A SOC analyst can detect these patterns and raise an alert.

## What I Learned

- How an attacker approaches a website step by step: find the target, discover hidden areas, then attack the weakest point.
- Why security teams need both an attacker's view (to understand threats) and a defender's view (to stop them).

## Next Steps

➡️ Continue the Pre Security path and move on to Defensive Security Intro.
