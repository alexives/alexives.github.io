---
layout: software
title:  "Play/Pause workflow for<br />Alfred 2"
date:   2015-07-28 14:16:42
categories: alfred code
author: Alex Ives
icon: images/play-pause/Play-Pause.png
repo: https://github.com/alexives/play-pause-alfred-workflow
latest_release: https://github.com/alexives/play-pause-alfred-workflow/releases/latest
---

For a long time, I've been using a variety of web streaming services. One of the biggest issues with it is this: When I walk away from my desk, I have to dig through all of my open browser tabs and figure out where to pause it.

That's where this workflow comes in.

This workflow utilizes the the Google Chrome Applescript api, which allows you to execute arbitrary javascript on a page. Based on a list of services, and the html class or id elements of their play/pause buttons, it looks through open browser tabs and will play or pause the music streaming service of your choice.

Currently it's implemented with bash wrapped applescript for the filtering, though I'm thinking about moving it to something a little bit more sane, like python. 