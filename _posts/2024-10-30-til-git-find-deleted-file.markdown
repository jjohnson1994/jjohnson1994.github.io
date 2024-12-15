---
layout: post
title:  Search git history for deleted files
date:   2024-10-18 18:29:04 +0100
categories: git, til
---

<i>So I don't forget:</i>

I needed to find when a file was deleted, turn out I could use the part of the file path I did knew to search the `git log`

``` bash
git log --all --full-history -- "**/pages/my-page/index.vue"
```

Nice!
