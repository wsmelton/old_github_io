---
layout: post
title: Visual Studio Community
permalink: /vs-community/
date: 2020-09-11 08:00
tags: [dbatools]
published: false
---

I have typed a good bit in the past year evangelizing about Visual Studio Code. It was not the first development tool I used for PowerShell. Contributing with <a href="https://dbatools.io" target="blank">dbatools</a> module I actually started out using the big brother Visual Studio 2015 Community Edition (referred to as just "VS"). The PowerShell extension in this editor is maintained by <a href="https://github.com/adamdriscoll/poshtools" target="_blank">Adam Driscoll</a>. VS is now at version 2017 and the <a href="https://marketplace.visualstudio.com/items?itemName=AdamRDriscoll.PowerShellToolsforVisualStudio2017-18561" target="_blank">PowerShell Tools for Visual Studio</a> has had a ton of improvements since I last used it. So I thought I would take you through how to get VS setup for contributing to a GitHub project. We will obviously use dbatools as the example. :grin:

It is only fair that since I have used VS before to give you both sides of the coin. I like VS and Code, it is just Code has become my go-to editor now. However, I would like to share what VS offers so you can make an educated decision on what editor you would like to use. You could say VS is the big bother to Code but it offers a completely different experience in developing PowerShell than Code does, so you cannot really compare them directly apples-for-apples. Once you get familiar with the interface and toolbars though, it becomes pretty easy to use.

### Install

I am not going to touch on installing VS itself as that can be pretty drawn out process to try and document here. You can see a pretty good walk-through on the install from <a href="https://youtu.be/R6dZJ-FEypk" target="_blank">this YouTube video on VS channel</a>.

One thing to just note is when you start the install of VS itself just go see a movie or something, it takes a while. At some point it will give you a prompt to select a workload and individual components, you can skip these if you want. Just close that window. When all is done you should see a screen that shows the below, you will just click on "Launch":



Next thing is to make sure you have the extensions needed for GitHub and PowerShell. You can go into Tools > Extensions and Updates. Then just do a search for the following two extensions and install them:

1. GitHub Extension for Visual Studio (created by: GitHub, Inc)
2. PowerShell Tools for Visual Studio (created by: Adam Driscoll).

### Versions

The remainder of this post and screenshots focusses on the following build of VS and each extension on my machine:

- Visual Studio Community 2017 - 15.3.3
- GitHub Extension for VS - 2.3.2.32
- PowerShell Tools for VS - 3.0.585

