---
title: "Crafting multiple ROP chains using format strings"
date: 2025-12-26
draft: true
description: "A complete guide to all available shortcodes for the Hugo Narrow theme"
tags: ["ROP", "Format Strings"]
categories: ["PWN"]
cover: "cover.webp"
---

## Code review

## Understanding the stack


```c
int num = 1;
printf("num = %d\n", num);
printf("11111%n\n", &num);
printf("num = %d\n", num);
```

```
d3bo$ gcc format_strings.c -o format_strings && ./format_strings

num = 1
11111
num = 5
```
