---
title: "Automating Docker"
date: 2018-12-12T08:00:00-06:00
draft: true
---

If you do something more than once it should be automated or scripted in a repeatable manner. You likely have heard this before, and it applies across various task that support commands being run via any scripting language.

Docker is no different and has been picking up speed. Many post I have seen folks show how to run individual commands to pull down images. Microsoft has started publishing beta releases of Windows Server, SQL Server and even PowerShell via Docker images. This mechanism gives you the opportunity to play with features more quickly than having to go through constant install and uninstall process.

The talk around town right now is SQL Server 2019 preview releases. So to pull the latest CTP release of SQL Server you would see the following commands be issued in a command prompt:

```
PS C:\> docker pull mcr.microsoft.com/mssql/server:2019-CTP2.2-ubuntu
PS C:\> docker run -p 1416:1433 -e "ACCEPT_EULA=Y" -e "SA_PASSWORD=P@ssword12345 -d mcr.microsoft.com/mssql/server:2019-CTP2.2-ubuntu
```

The output of the pull command will look something like this:

![](/img/dockerctppull.png)

The second command starts a new container and output of this is:

![](/img/dockerrun.png)

The output includes use of the `docker logs` command where I can see SQL Server starting up to know when it is ready.

Once it starts up and accepts connections I can make a connection using SSMS or command line scripts. The server will be `localhost,1416` with the associated `sa` login and password set.

## Repeatable and automated

All of the above is nice but it is so time consuming to do this each time I want to get a full ~~development~~ playground up and running as a new CTP version is released.

