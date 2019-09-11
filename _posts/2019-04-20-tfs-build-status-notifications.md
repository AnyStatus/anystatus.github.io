---
layout: post
title:  TFS Build Status Notifications
redirect_from: "/2017/05/05/tfs-and-vsts-notifications.html"
date:   2019-04-20 11:00:00
author: Alon Amsalem
---

Still using email notifications from your TFS server? Download AnyStatus and start getting build notifications directly to your desktop.

## What is AnyStatus?

AnyStatus is a lightweight desktop application for Windows that brings together metrics and events from various sources into one simple dashboard. Examples include, Team Foundation Server, Azure DevOps, Jenkins, TeamCity, AppVeyor, Health Checks, Databases, Operating System Metrics and [more](/docs/plugins). A system tray icon is used to show the overall status. It's also available as Visual Studio extension. [Learn more](/)

## TFS Build Status Notifications

AnyStatus provides and easy way to visualize the status and progress of TFS builds on one or more TFS servers.
You can queue new builds straight from the dashboard. When a build status is changed, a desktop notification is displayed to alert the new status. You can also customize the status notifications or setup custom actions using AnyStatus triggers.

## Getting Started

To get build status notifications from TFS, download and install AnyStatus from our [Downloads](/downloads) page.
Launch AnyStatus from the Windows Start Menu and use the <i class="fas fa-plus"></i> button to add a new widget to the dashboard. Alternatively, you can use the *Context Menu > Add Widget* option.
Next, in the Add Widget Wizard select the **DevOps** category and then **TFS Build** widget.

1. Enter a name for the widget.
2. Enter the TFS server URL. For example: http://tfs:8080/tfs
3. Enter the Collection name (default is DefaultCollection), the Team Project name and Build Definition name.
4. Click **Test** to run the widget, any error messages are logged in the Activity Log.
5. Click **Add** to save the new widget in the dashboard.

<img src="/assets/posts/2017-05-05-tfs-and-vsts-notifications/add-tfs-build-monitor.png" class="img-fluid" alt="TFS Build Status Notifications"/>

![AnyStatus 2.4.36 & Azure DevOps Plugins](/assets/images/screenshots/anystatus-2.4.36-azure-devops.png)<br/><small>AnyStatus Desktop 2.4.36 with Azure DevOps Plugins</small>

AnyStatus will start monitoring the newly created widget immediately.
Any errors or warnings that may occur will be logged in the Activity Log.
When the status of your TFS build change, a desktop notification will popup showing the new build status.

## Queue new build

Once the widget has been created, you can queue new builds using the *Context Menu > All Tasks > Start* option.

## Reconcile workspace after successful builds

You can automatically reconcile your workspace after a successful build using [Triggers](/docs/triggers), a feature that enables you to run custom commands, such as [tf.exe reconcile](), when statuses change.
