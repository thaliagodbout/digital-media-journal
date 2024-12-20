---
title: Multiplayer Computational Sketching
created: 2024-11-14
last_modified_at: 2024-11-14
---

<div class="overview">
Brief thoughts and notes from turning Curly into a collaborative environment.
</div>

During class, we worked on making our Curly reproduction collaborative so that people can interact together online.

**Some notes from node.js:**
- Automatically generating package.json file for dependencies
- Separating client-side files in a folder
- Using web sockets to send messages between client and server

**For Yellowtail:**
- When a person draws a line, on pointerup, we send the list of paths to the server
- Callbacks/event listeners to run code whenever new messages are received/when new clients connect to the server

I don't have many notes on this, but I'm curious about creating real-time collaborative virtual worlds - how might we co-create our virtual microworlds together by bringing collaboration into them?