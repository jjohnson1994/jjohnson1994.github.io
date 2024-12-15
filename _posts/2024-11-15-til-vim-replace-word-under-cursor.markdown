---
layout: post
title:  VIM Substitute word under cursor
date:   2024-11-15 08:19:00 +0000
categories: TIL, VIM
---

<i>TIL</i> you can use the current word registor with `:s` (or `:substitute`) to quickly substitute the word under the cursor.

example:
`:%s/<C-r><C-w>/2025/g`

This command with replace all instance of the word under the cursor with '2025'.

In command mode `<C-r>` inserts text from a register and `<C-w>` references the word under the cursor
