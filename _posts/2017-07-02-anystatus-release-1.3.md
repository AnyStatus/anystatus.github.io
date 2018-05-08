---
layout: post
title:  AnyStatus Release 1.3
date:   2017-07-02 12:00
author: AlonAm
tags: [New Releases]
---

The latest release of AnyStatus includes the new open source [API](https://github.com/anystatus/api) and [Plugins](https://github.com/AnyStatus/Plugins) code libraries. You can now improve existing plugins, add new ones or even create your own private plugins library.

The open source projet is licensed under AGPL open source license, if that is an issue for you, please leave a feedback.

This release also includes a new SQL Query plugin and other features and improvements.

## In this post
---------------

- [AnyStatus API and Plugins open source libraries](#anystatus-api-and-plugins-libraries)
- [AnyStatus plugins library](#anystatus-plugins-library)
- [Improved "Add new item" window](#new-add-new-item-window)
- [SQL Query Plugin](#sql-query-plugin)
- [Bypass Monitors](#bypass-monitors)
- [Other Changes](#other-changes)

## AnyStatus API and Plugins Libraries
----------------------------

AnyStatus API and Plugins libraries are now open source and can viewed by users who wish to know more about certain plugins.

Each plugin contains the attributes that tells AnyStatus how and where to show the plugins in the dashboard.

In addition, plugins are using API interfaces to add functionality and behaviours such as triggering a build and restarting a service.

You can also develop plugins that are not monitored such as a to-do item, a URL shortcut or even start a program.

Plugins and extensions are automatically discovered at startup. AnyStatus scans assemblies in the installation directory who's name starts with *AnyStatus*.

Developers are invited to add new plugins to the library or suggest improvements and bug fixes by creating pull requests.


## New "Add new item" window
----------------------------

The "Add new item" window have slightly changed to make it more clean and simple.
The monitors list is now showing one group at a time and the menu look and colors have changed too, I hope to improve color contrast in next releases.
Your feedback about colors and usability is highly appreciated.

![Add new item](/assets/posts/2017-07-02-anystatus-release-1.3/add-new-item.png)


## SQL Query Plugin
-------------------

The SQL Query plugin enables you to enrich the dashboard with queried data from any external Microsoft SQL Server database.

![SQL Query Plugin](/assets/posts/2017-07-02-anystatus-release-1.3/sql-query-plugin-demo.png)

![SQL Query](/assets/posts/2017-07-02-anystatus-release-1.3/sql-query-plugin.png)


## Check for updates
--------------------

Another new feature was added which checks for new versions during startup. In this version the new version details are shown in the activity log and
in future versions, AnyStatus will show a desktop notification or notify you from within Visual Studio.
The feature can be enabled or disabled in the options window.

## Bypass Monitors
------------------

You can now bypass monitors by specifying an interval of 0. When monitors are bypassed, AnyStatus checks for the status once and every time you click the "Refresh" button.

## Other Changes
---------------------

In this release, I have simplified the desktop notification messages text and I am always looking for ways to improve it, feel free to suggest changes.
I have also removed a few  unused assemblies to reduce the installation package size and improved assembly scanning to reduce startup time.


## Summary
----------

That’s it for now. I hope you enjoy the latest features and imrovements. Feel free to leave a comment and let me know what you think!
