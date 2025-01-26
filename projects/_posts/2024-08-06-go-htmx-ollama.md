---
layout: post
title: "Golang + HTMX + Ollama Chatbot"
date: 2024-09-15 23:32:31 -0400
tags: golang ollama htmx
image: /assets/images/htmx-ollama.png
excerpt: "My first Go project!"
repo: https://github.com/zhichen-guo/go-ollama-htmx-chat
---
![App Screenshot]({{ page.image | relative_url }})

This summer has been all about exploring the capabilities of LLMs. At work, we've been playing with open source models using Ollama – building RAG apps with ChromaDB, Python (FastAPI), and React.

Outside of work though, I've been really curious about exploring other languages – particularly Golang – and going back to building monolithic, server-side rendered apps (my first web framework was Ruby on Rails). So building a Go RAG application seemed like the perfect project. I also decided to try out HTML - very much inspired by ThePrimeagen.

I tried to use the Go http server I wrote from scratch following a tutorial by CodeCrafters, but gave up and used the standard `net/http` package instead. I did, however, handle my own templating using the built-in `os` and `fmt` packages instead of a dedicated template engine.

HTMX was also a very cool tool to use. And for a simple app that didn't need very dynamic UI elements, it did the job perfectly.

I'm still trying to wrap my head around working with Go, but I'm excited to continue learning.