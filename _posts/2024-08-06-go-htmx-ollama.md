---
layout: post
title:  "Golang + HTMX + Ollama Chatbot"
date:   2024-09-15 23:32:31 -0400
tags: golang ollama
---

This summer has been all about exploring the capabilities of LLMs, especially in RAG applications. At work, I've built RAG-powered chats using Streamlit and FastAPI + React, Ollama, and ChromaDB.

But since I recently started learning Golang, and as a throwback to my first web-dev days in full-stack Rails, I challenged myself to create a chat UI using Golang and HTMX.

This was a great project to get a feel for Go's `net/http` package, as I got to handle client requests and also create requests to the Ollama API. I also got to create a rough templating system by using the `os` and `fmt` packages to read in plaintext files with string formatters. 

Using HTMX was also a very cool experience. It was a very welcomed break from React dominance and a very refreshing throwback to  the monolithic full-stack applications that started my webdev journey. I found the triggers and swaps very intuitive, and I loved how easy it was to put together a nice-looking UI with a bit of dynamism.

I'm still trying to wrap my head around writing Go code, but it's forcing me to be much more mindful of things like project structure, variable types, and error handling. I'm excited to continue learning Go to create more web applications and exploring some CLI packages as well!

![App Screenshot](/assets/htmx-ollama.png)