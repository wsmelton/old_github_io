---
layout: post
title: Visual Studio Community
permalink: /vs-community/
date: 2017-12-01 08:00
tags: [dbatools]
published: false
---

I have typed a good bit in the past year evangelizing about Visual Studio Code. Contributing with <a href="https://dbatools.io" target="blank">dbatools</a> module I actually started out using the big brother Visual Studio 2015 Community Edition (referred to as just "VS"). The PowerShell extension in this editor is maintained by <a href="https://github.com/adamdriscoll/poshtools" target="_blank">Adam Driscoll</a>. VS is now at version 2017 and the <a href="https://marketplace.visualstudio.com/items?itemName=AdamRDriscoll.PowerShellToolsforVisualStudio2017-18561" target="_blank">PowerShell Tools for Visual Studio</a> has had a ton of improvements since I last used it. In this post I thought I would take you through getting VS 2017 installed and setup for PowerShell development. I will also go over how to get VS setup for contributing to a GitHub project. We will obviously use dbatools as the example repository. :grin:

### Install

_One thing to just note: when you start the install of VS itself just go see a movie or something as it takes a while._

First step is to download the installer from [here](https://visualstudio.com/free-developer-offers). I will walk through the installation for Visual Studio Community.

The following will be the order of screens/prompts you will get on the installation (at least at current date):

Click continue

![](/img/vs-install_1.png)

![](/img/vs-install_2.png)

At this point you are prompted to select a workload and individual components. You can go through and select the ones you desire, but I am opting to skip this process right now. (Adding more workloads does add on time for the install process).

![](/img/vs-install_3.png)

After a bit you will see a screen show the installation progress:

![](/img/vs-install_4.png)

Once that is completed you can click on "Launch" button:

![](/img/vs-install_5.png)

One final step before VS opens is to sign into your Live account, this is primarily utilized for VSTS and other various services associated with it.

![](/img/vs-install_6.png)

![](/img/vs-install_7.png)

You should now be presented with something similar to this:

![](/img/vs-install_8.png)

### Extensions

Now that we have VS installed we will need to add some extensions before we can develop with PowerShell. There are only two extensions needed:

1. GitHub Extension for Visual Studio (created by: GitHub, Inc)
2. PowerShell Tools for Visual Studio (created by: Adam Driscoll).

Start going to Tools > Extensions and Updates...

![](/img/vs-install_9.png)

(1) Select "Online", (2) Search for "PowerShell" then (3) select "PowerShell Tools for Visual Studio" and click Download

![](/img/vs-install_10.png)

Then perform the same steps for "GitHub"

![](/img/vs-install_11.png)

Once that download completes you can close that window, and then exit out of Visual Studio. It will vary but after a few seconds you will se the VSIX Installer open up and being installing the extensions.

It will first initialize and then give you a prompt to click "Modify" for the install to continue:

![](/img/vs-install_12.png)

![](/img/vs-install_13.png)

On my machine the install of the PowerShell extension took close to a full hour. Once the extensions install are complete, just click "Close":

![](/img/vs-install_14.png)

### Versions

The remainder of this post and screenshots focusses on the following build of VS and each extension on my machine:

- Visual Studio Community 2017 - 15.4.5
- GitHub Extension for VS - 2.3.6.391
- PowerShell Tools for VS - 3.0.585

