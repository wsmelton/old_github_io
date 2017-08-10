---
layout: post
title: Debugging in PowerShell
subtitle: A field of issues to solve
permalink: /debugging-powershell
date: 2017-08-07 02:00
tags: [powershell,vscode]
bigimg: /img/fly-swatter-149265_640.png
---

## The what and why

Debugging code can be eventful to simply figure out why something works the way it does. As well, in the age of "everything is a module" in PowerShell we can't discount finding out what a function or command does. 

The more you know the easier it is to debug when an issue occurs. Especially if you are the author of that code.

The main way you can do this in debugging is by using an IDE that allows you to more easily interact with the debugging service for PowerShell.

## Tools

I am an avid user of [Visual Studio Code](https://code.visualstudio.com) (VS Code). It offers the ability to have a UI when you debug PowerShell code. If you have ever used [the ISE to debug PowerShell scripts](https://docs.microsoft.com/powershell/scripting/how-to-debug-scripts-in-windows-powershell-ise), then are have a good head start in using VS Code.

## Real use-case

So in showing you how to debug, I thought it would be helpful to try and walk you through an true-to-life use case that I worked on this past week.



Header image provided via [pixabay](https://pixabay.com/en/fly-swatter-flyswatter-fly-flap-bug-149265/)