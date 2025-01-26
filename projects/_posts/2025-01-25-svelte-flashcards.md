---
layout: post
title: "Svelte Flashcard App Template"
date: 2025-01-25 00:00:00 -0400
tags: svelte
image: /assets/images/flashcard-thumbnail.png
excerpt: "A reusable, db-less flashcards webapp"
repo: https://github.com/zhichen-guo/svelte-flashcard-template
---
![Svelte Flashcards App Video]({{ "/assets/images/flashcards-video.gif" | relative_url }})

Recently I started playing piano again, and wanted to create a flashcards app to help me learn chords and II-V-I progressions in Jazz. I thought before I made the app Jazz-specific, it would be better to make a generic flashcards webapp that can be repurposed for all sorts of things.

This app is build using Vite, Svelte, and TailwindCSS. It was my first time using both Svelte and TailwindCSS. I really enjoyed all the features that Svelte + SvelteKit had to offer, from animations to server-side functions to the straightforward routing system. In terms of Tailwinds, my initial worry about cramming all of those class names into the HTML didn't turn out to be as bad as I thought.

This flashcard app doesn't rely on any DB. All the card sets are stored as JSON in the codebase. This saved me from all the complexity of using an ORM and dealing with admin accounts, while still giving me the flexibility of easily creating new flashcards sets as needed. It also supports flashcards with both text and images.