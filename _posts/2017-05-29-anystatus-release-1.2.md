---
layout: post
title:  AnyStatus Release 1.2
date:   2017-05-28 12:00
author: AlonAm
tags: [New Releases]
---

AnyStatus 1.2 has been released to the official [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=AlonAmsalem.AnyStatus) with a few new features and bug fixes.
This release is focused around [AnyStatus Desktop](#anystatus-desktop) and the Dynamic Source Code monitor that lets you to write your own custom monitors using C# or VB.NET code.

## In this post
---------------

- [AnyStatus Desktop](#anystatus-desktop)
- [Jenkins Job Progress Bar](#jenkins-job-progress)
- [Custom Monitors](#custom-monitors)
- [SQL Server Connection](#sql-server-connection)
- [Network Speed](#network-speed)
- [IIS Application Pool](#iis-application-pool)
- [Minor Changes](#minor-changes)
- [Bug Fixes](#bug-fixes)
- [New Website](#new-website)


## AnyStatus Desktop
--------------------
AnyStatus Desktop is a standalone version of the Visual Studio extension that shares the same codebase, user interface and features to bring the best of AnyStatus to non Visual Studio users. The standalone version also significantly improves the development and debugging process of AnyStatus and opens the door for other features like supporting high-contrast themes and more.

AnyStatus Desktop comes as a separate installer and will be available for download soon.

![AnyStatus Desktop](/assets/posts/2017-05-29-anystatus-release-1.2/anystatus-desktop-1.2.png)


## Custom Monitors
------------------
Introducing the first version of Dynamic Source Code monitor that lets you write custom monitors in C# or VB.NET files. The source code is built on the fly and recompiles when needed. Compilation warnings and errors are redirected to the output window.

Writing custom monitors is the same as writing a console application.
The C# or VB.NET file must have a class or a struct with a static `Main()` or `Main(string[] args)` method.
The `Main()` method can return `void` or `int` to control the status of the monitor.
Assmebly references and the arguments that are passed to the `Main(string[] args)` method can be configured through the UI.

More on custom monitors in a separate blog post.

## Jenkins Job Progress
-----------------------
Jenkins jobs are now showing a progress bar when the job is running. Note, the width of the progress bar is dynamic. I wasn't sure about this but since it looks good on the UI, I've decided to keep it. If you think it should be fixed please let me know in the comments section below.

![AnyStatus Desktop](/assets/posts/2017-05-29-anystatus-release-1.2/progress-bars.png)


## Network Speed
---------------- 
You can now view the Upload and Download speed of your network interfaces.
The speed is measured for 1 second every monitor check and displayed in Kbps or Mbps.

![AnyStatus Desktop](/assets/posts/2017-05-29-anystatus-release-1.2/network-speed.png)


## SQL Server Connection
------------------------
SQL server connection monitor lets you monitor a connection string to make sure it can be opened.
The database connection is opened and closed immediately every check.


## IIS Application Pool
-----------------------
Monitor the state of local and remote IIS application pools. Note, this monitor uses the [ServerManager](https://msdn.microsoft.com/en-us/library/microsoft.web.administration.servermanager(v=vs.90).aspx) class which requires you to be an administrator on the remote machine and you can't specify a different user name and password. I hope to find better ways to monitor and control (start, stop, recycle) remote application pools in future versions.


## Minor Changes
----------------
- You can now specify the expected exit code of PowerShell and Batch scripts
- Added a new toolbar button tp open AnyStatus activity log in the Visual Studio output window
- Custom actions like “Open in browser” and “Trigger a new build” are now disabled when the status is Error
- Bold folder names


## Bug Fixes
------------
- Fixed VS crash when dragging an item in the tree-view while it is being edited
- Fixed VS crash when opening the Options page after first installation before opening the tool window


## New Website
--------------
AnyStatus website also got some love this week. If you spot any broken links or pages that look off, let me know!
This website is powered GitHub pages, which means you can fork it and create pull-requests if you'd like to help me improve it.


## Summary
----------
That's it for now. I hope you enjoy the latest features. Feel free to leave a comment and let me know what you think!


