---
title: Playing TapMe.plus in the Browser
subtitle: The web version is for quick access, while the homepage stays lightweight.
permalink: /posts/browser-puzzle-game/
tags:
  - browser puzzle game
  - web game
  - WebAssembly
  - no download
---

TapMe.plus can run in the browser, which makes it easy to try the game without installing anything first.

The official site stays lightweight. It does not embed the game on the homepage anymore, because loading a Godot WebAssembly build should be an intentional action. When you click Play, the dedicated web game opens and downloads the runtime and game package there.

## Why the first load can take longer

A browser game made with Godot is not the same as a normal article page. The first launch needs the game runtime, data package, and supporting files. That can take a little time, especially on mobile networks.

After that, the browser can cache the files. Later visits are usually faster.

## Good for trying the core loop

The web version is a good way to feel the TapMe.plus rule quickly:

- tap a tile to add 1;
- connect three or more matching numbers;
- watch the board drop;
- chase the next chain.

If the game clicks with you in the browser, the same core logic carries over to iPhone and iPad.

## A practical note

If the web game stalls, try a modern browser such as Safari, Chrome, Edge, or Firefox, and make sure your network is not blocking large WebAssembly files.

The game is simple to play, but the web build is still a real game package.
