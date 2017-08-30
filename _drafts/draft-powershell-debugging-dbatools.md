---
layout: post
title: Debugging dbatools
subtitle: A field of issues to solve
permalink: /debugging-powershell
date: 2017-08-07 02:00
tags: [dbatools]
bigimg: /img/fly-swatter-149265_640.png
---

## Keeping it Real

I thought it would be helpful to walk you through a true-to-life scenario that I had where I needed to debug the [dbatools module](https://dbatools.io). An [issue](https://github.com/sqlcollaborative/dbatools/issues/2012) was filed on the repository that pointed out in certain cases multiple login failed messages are written to the SQL Server instance passed into a command when a credential is provided. The login failure is generally showing as the Windows account running the PowerShell session (_powershel.exe_). The issue noted that in this case the environment did not allow the Windows account access to the SQL Server instance, hence the need to pass in a SQL Credential (or SQL Login).

The conundrum came in that this was not with every command. In this issue the user was using `Test-DbaIdentityUsage` and if he used `Get-DbaDatabase` he didn't see the same issue.

Header image provided via [pixabay](https://pixabay.com/en/fly-swatter-flyswatter-fly-flap-bug-149265/)