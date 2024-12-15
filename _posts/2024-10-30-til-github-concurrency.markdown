---
layout: post
title:  Github concurrency
date:   2024-10-18 18:29:04 +0100
categories: github-actions
---

annoying github actions thing

> GitHub Workflow error: Canceling since a higher priority waiting request for

🤔

We wanted to queue our e2e runs. This was to mitigate the chance of one run distrupting another, as (for now) each run shares the same backend.

Easy! We can use a concurrency group to queue jobs. Nope... turns our concurrency group cancel any pending tasks in favor of newer ones

https://github.com/orgs/community/discussions/41518

