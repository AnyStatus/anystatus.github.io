---
layout: post
title:  TFS Build Status Notifications
redirect_from: "/2017/05/05/tfs-build-notifications.html"
date:   2017-05-05 10:00:00
author: Alon Amsalem
---

Still using email notifications from your TFS server? Download AnyStatus and start getting build notifications directly to your desktop.

#### Overview

AnyStatus is a lightweight desktop notifications app designed to show statuses of various CI/CD tools such as Team Foundation Server, Azure DevOps, Jenkins, TeamCity and AppVeyor, all in a single dashboard. These include, builds, releases, jobs, deployment environments, work items and more. In addition to CI/CD pipelines, AnyStatus provides basic monitoring capabilities to monitor the health state and availability of deployment environments.<br/>AnyStatus is available as desktop application for Windows or Visual Studio extension. [Learn more](/)

#### Get TFS Build Status Notifications

To get build status notifications from TFS on your desktop, download and install AnyStatus from our [downloads](/downloads) page.<br/>
Use the + button to add a new TFS Build widget to AnyStatus dashboard. Alternatively, use the Context Menu > Add Widget option.<br/>

![AnyStatus 2.4.36 & Azure DevOps Plugins](/assets/images/screenshots/anystatus-2.4.36-azure-devops.png)<br/><small>AnyStatus Desktop 2.4.36 with Azure DevOps Plugins</small>

In the Add Widget window select the DevOps category and then TFS Build.

![TFS Build Notifications](/assets/posts/2017-05-05-tfs-and-vsts-notifications/add-tfs-build-monitor.png)

Enter a name for the widget. Enter the TFS server URL. For example: http://tfs:8080/tfs. Enter the collection name (default is DefaultCollection) the team project name and build definition name. Click Add to save the new widget. AnyStatus will start monitoring the newly created widget immediately. Any errors that may occur will be logged in the activity log. Once the widget has been added. You can queue new builds using the Context Menu > Tasks > Start option.

#### Reconcile workspace after a successful build

Use [triggers](/docs/triggers) to automatically reconcile workspace after a successful build.
