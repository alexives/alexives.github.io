---
layout: software
title:  "An Eclipse Workflow for Alfred 2"
date:   2015-5-2 10:30:42
categories: alfred ide
icon: images/eclipse.png
latest_release: /files/Eclipse.alfredworkflow
---
Like some other eclipse users, I maintain multiple workspaces to avoid distractions on other projects. Anything from opening similarly named classes across projects to simply getting distracted by things I'd rather be doing, keeping some of my workspaces isolated is useful to me. The biggest issue then is when I do want to swtich back and forth between open workspaces. There are plugins for eclipse for this, and a while ago I rolled my own helper scripts to open eclipse from an iTerm session. 

The issue with opening it in an iTerm session is this: If I close that iTerm window it shuts down eclipse. This was very annoying to me. I could have solved this by using an eclipse plugin that lets you open a second workspace once eclipse was open, but that doesn't solve everything. When I first open eclipse, I hate having to wait for it to open the stupid popup window asking which workspace I want. I want to open eclipse, go do something else while it loads, and then go back to a ready to go eclipse. 

![Workspaces from alfred]({{site.baseurl}}/images/alfred-eclipse/eclipse-workspaces.png)
More recently I switched to using [Alfred 2](http://alfredapp.com) as my quick launch on OS X. After months of using it I finally bought the paid version that let's you make custom workflows (read plugins) to automate various tasks. To that end, I spent a little time putting together a workflow that lets me jump straight to an eclipse workspace. The concept is simple. It looks for an instance of eclipse using mdfind, and looks at the settings file for a list of workspaces I've opened in the past. The one downside is if I had workspaces I've never opened this won't find them, but for the most part that's a sort of one off scenario and I decided I didn't care.