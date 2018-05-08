---
layout: post
title:  TFS and VSTS Build Notifications
redirect_from: "/2017/05/05/tfs-build-notifications.html"
date:   2017-05-05 10:00:00
author: AlonAm

---

AnyStatus is a lightweight Visual Studio extension and Windows application that you can use to monitor the status of your builds, releases, servers, network and remote services on the back end of your development workflow.

With AnyStatus, you can monitor builds and releases on [Visual Studio Team Services](https://www.visualstudio.com/team-services/) and [Microsoft Team Foundation Server](https://www.visualstudio.com/tfs/).

![TFS Build Notifications](/assets/posts/2017-05-05-tfs-and-vsts-notifications/tfs-build-monitor.png)

To add a TFS build monitor to AnyStatus dashboard, open the "New Item" dialog using the toolbar or context menu and select **Continuous Integration > TFS Build**.

![TFS Build Notifications](/assets/posts/2017-05-05-tfs-and-vsts-notifications/add-tfs-build-monitor.png)

Enter the name of the monitor, the URL address of your TFS server or VSTS account.

For VSTS: https://**your-account**.visualstudio.com

For TFS: http://server:port/tfs

Enter the Collection, Team Project and Build Definition names.
Optionally you can spceificy user name and password or leave them empty for windows authentication.

Once the monitor has been created, you can trigger a new build or open the build web page in your default browser.

![Trigger TFS Build](/assets/posts/2017-05-05-tfs-and-vsts-notifications/tfs-trigger-build.png)


**Edit:** A new VSTS plugin for monitoring builds and releases has been release in AnyStatus 1.4.66. The new plugin supports Personal Access Tokens.
