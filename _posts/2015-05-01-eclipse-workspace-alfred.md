---
layout: post
title:  "An Alfred 2 Workflow for Eclipse Workspaces"
date:   2015-1-3 10:30:42
categories: alfred ide
---

A few months ago, I switched from using OS X's built in product spotlight to [Alfred 2](http://www.alfredapp.com/), which is a thrid party tool along the same lines. There were a number of reasons that I switched. The biggest issue I aways had with spolight was the Calculator. I know it may sound silly but the way the calculator works in spolight is pretty much the worst. So you type an expression like 90*2.125 (2 1/8 Inches at 90 ppi), and it shows you the answer is 191.25. This sounds good, that's the right answer after all. This is wehre the problem starts though. Up until here, Alfred and Spotlight behave pretty similarly. The difference is when you hit enter. If you're like me, you expect something useful to happen, like copy the answer to your cliboard or something (which is precisely what Alfred does), but no, it opens the calculator app. So, that's not so bad right, at least it puts the expression from spotlight into your calculator so you COULD copy the answer, right? Wrong. It opens an empty calculator app.

At any rate, if my feelings about spotlight in this manner aren't clear at this point, let me help. Spotlight is a bold idea that does some great things, but has enough minor frustrations that it makes me want to beat my head against the wall. A friend of mine showed me [Flashlight](https://github.com/nate-parrott/Flashlight) which does solve some issues, like extensability. The fact that there isn't a built in way to extend the spotlight interface is yet more reason to feel for other products.

So, back to alfred. For the first 6 months, I mostly ignored the paid version of Alfred 2 (called the powerpack). About a week ago, I finally realized what I was missing. Alfred allows for you to create custom workflows that are manageable and relatively easy to use. With that in mind, I realized there was something I'd always wanted and never had. Like some other eclipse users, I need to manage multiple workspaces. Too many projects in one workspace has always been an issue for me. So instead, I tend to have multiple workspaces. This of course means that I have to tell it which one to launch every time I start.

In response to that, I built myself a workflow that would open eclipse workspaces for me. It works by pulling the list of workspaces out of your eclipse preferences, and then regexs against the names with fuzzy matching so that you can open 

#### [Download it here]({{site.baseurl}}/files/Eclipse.alfredworkflow)