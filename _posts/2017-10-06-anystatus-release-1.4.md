---
layout: post
title:  AnyStatus Release 1.4
date:   2017-10-06 12:00
author: AlonAm
tags: [New Releases]
redirect_from: "/2017/07/02/anystatus-release-1.4.html"
---

AnyStatus 1.4 has been released with a few new features and bug fixes.
In this blog post, I'll review some of the features and changes in this release.


## In this post
---------------

- [View the overall status in system tray](#view-the-overall-status-in-system-tray)
- [New VSTS Plugins](#new-vsts-plugins)
- [Jenkins View](#jenkins-view)


## View the overall status in system tray
-----------------------------------------

The new system tray icon in AnyStatus Desktop now reflects the overall status of all monitors in the dashboard.
Each status is represented by a different icon. The status description is shown in the icon tooltip.

![AnyStatus Tray Icon](/assets/posts/2017-10-06-anystatus-release-1.4/anystatus-tray-icon.png)

<br/>

Here is a short demo of the new icon in action

![AnyStatus Tray Icon](/assets/posts/2017-10-06-anystatus-release-1.4/anystatus-tray-icon.gif)


## New VSTS plugins
-------------------

Release 1.4 includes two new plugins for VSTS

* VSTS Build
* VSTS Release

The VSTS Build plugin is the same as the TFS Build plugin but with support for Personal Access Tokens.

The new VSTS Release plugin shows the overall status of releases with separate node for each deployment environment.
This plugin is based on a new capability which enables plugins to add other plugins in run-time.

![VSTS Release](/assets/posts/2017-10-06-anystatus-release-1.4/vsts-release.png)


## Jenkins View
---------------

Another new plugin, contributed by Alexander Kolky, is the Jenkins View plugin.
Alexander came up with a really cool idea, to scan and add Jenkins Jobs at runtime.

With this plugin, you no longer need to add Jenkins Jobs one by one, you can add an entire view into your dashboard.
AnyStatus will automatically scan and add jobs within the view.

Whenever a job is added or removed, AnyStatus will automatically update your dashboard.
Each one of the jobs within the view is a Jenkins Job plugin which you can trigger or refresh independently.

The plugin supports Jenkins pipeline and multibranch jobs too.


