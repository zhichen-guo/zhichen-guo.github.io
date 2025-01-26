---
layout: post
title: "Grappling Hook"
date: 2025-01-13 00:00:00 -0400
tags: svelte
image: /assets/images/grappling-hook.png
excerpt: "A small bash script to simplify repo navigation"
repo: https://github.com/zhichen-guo/grappling-hook
---
![Grappling Hook]({{ page.image | relative_url }})

While navigating through projects in the terminal, I always wished there was a way to just return to the root directory of the project without having to think so much about how many `..`s to use in your `cd`. Sort of like a `cd -` but a bit smarter. That was the inspiration for this project.

All it is is just a shell script that keeps going up from your working directory to its parent directories until it finds one with a `.git` subdirectory. Since a shell subprocess cannot perform `cd`s, the script only `echo`s the right directory and you must add a function in your bash file to `cd` using the output of the shell script. In my case I named this function `hook`.

![Hook command]({{ "/assets/images/hook.png" | relative_url }})

In addition to just taking you to the parent directory with a `.git` subdirectory, you can also pass an extra variable equal to the name of a directory in the path from your working directory to the parent directory to be `cd`'d into that directory instead.

![Hook command with argument]({{ "/assets/images/hook-with-argument.png" | relative_url }})