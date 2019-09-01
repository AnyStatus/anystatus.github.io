---
layout: post
title:  Monitor Jenkins jobs using AnyStatus
date:   2017-04-22 11:00:00
author: AlonAm
---

AnyStatus is a lightweight desktop application for Windows that brings together metrics and events from various sources. Examples include CI/CD processes, pull requests, work items, health checks, operating system metrics, and more. Think of it as CCTray on steroids. It's also available as a Visual Studio plugin.

AnyStatus enables developers to monitor and trigger [Jenkins CI](https://jenkins.io/) jobs and get notified about status changes.

![Jenkins Build Notifications](/assets/posts/2017-4-22-jenkins-build-notifications/jenkins-build-monitor.png)

To create a Jenkins job monitor, open the "New Item" dialog in AnyStatus using the toolbar or context menu and select **Continuous Integration > Jenkins Build**.

![Jenkins Build Notifications](/assets/posts/2017-4-22-jenkins-build-notifications/add-jenkins-job-monitor.png)

Enter the name of the monitor and the URL address of the Jenkins jobs.
For example: https://ci.jenkins.io/job/Core/job/jenkins/job/master/

You can specify a user name and API token or leave it empty to access Jenkins anonymously.
The API token is available in your personal configuration page. Click your name on the top right corner on every page, then click "Configure" to see your API token.
(The URL $root/me/configure is a good shortcut.) You can also change your API token from there.

Once the Jenkins monitor has been created, you can right-click the monitor to open the context menu and select **Trigger a new build** to start the job or **Open in Browser** to open the Job web page in your default browser.

![Jenkins Build Notifications](/assets/posts/2017-4-22-jenkins-build-notifications/jenkins-trigger-build.png)
