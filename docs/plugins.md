---
layout: docs
title: AnyStatus Plugins
---

AnyStatus is an extensible Windows application that rolls up metrics and events from various sources into one simple dashboard. Examples include builds and releases, health checks for different services and operating system metrics.
Check out the [API Documentation](/docs/api) to learn more about AnyStatus extensions and plugins.

## Azure DevOps Plugins
-----------------------
Quickly view and control the status of your CI/CD Builds, Releases, Deployment Environments and Work Items on [Azure DevOps Services](https://azure.microsoft.com/en-us/services/devops/). The Azure DevOps extension pack is a separate installation that adds new widgets with additional features that are not available in the free open source widgets. These include, history, progress and estimated time remaining of builds and release. Custom work item queries, and more. Support us by purchasing a license!

For more information and inquiry please [contact us](mailto:info@anystat.us).

<p>
    <form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_top">
        <button class="btn btn-warning" onclick="ga('send', 'event', 'Buy', 'Azure DevOps');">Buy Now</button> 
        <input type="hidden" name="cmd" value="_s-xclick">
        <input type="hidden" name="hosted_button_id" value="DSSVLGELMML32">
        <img alt="Buy Now" src="https://www.paypalobjects.com/en_US/i/scr/pixel.gif" width="1" height="1">
    </form>
</p>

## Open Source Plugins
----------------------
These are the default pre-installed widgets that comes free with AnyStatus. The source code is open for modifications and available on [GitHub](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/DevOps/TFS/Build). C# developers are invited to make changes and submit pull requests to help us maintain a free and open source set of tools for everyone to use.

**DevOps**

- TFS Build ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/DevOps/Microsoft/TFS/Build))
- Azure DevOps Build ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/DevOps/Microsoft/VSTS/Build))
- Azure DevOps Release ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/DevOps/Microsoft/VSTS/Release))
- Jenkins Job ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/DevOps/Jenkins/Job))
- Jenkins View ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/DevOps/Jenkins/View))
- AppVeyor Build ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/DevOps/AppVeyor/Build))
- TeamCity Build ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/DevOps/TeamCity/Build))
- Coveralls Code Coverage ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/DevOps/Coveralls))

**Health Checks**

- Windows Service ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/HealthChecks/WindowsService))
- HTTP/S ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/HealthChecks/HTTP))
- TCP/UDP ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/HealthChecks/PortCheck))
- Ping ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/HealthChecks/Ping))
- SQL Server Connection ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/HealthChecks/SqlServer/Connection))
- IIS Application Pool ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/HealthChecks/IIS/AppPool))
- Uptime Robot ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/HealthChecks/UptimeRobot))
- Pingdom ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/HealthChecks/Pingdom))

**Metrics**

- CPU Usage ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/Metrics/CPU/Usage))
- 8*New!** Battery ([Source](https://github.com/AnyStatus/Plugins/blob/master/src/AnyStatus.Plugins/Widgets/Metrics/Battery/BatteryStatusQuery.cs))
- Performance Counter ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/Metrics/PerformanceCounters))
- SQL Scalar Query ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/Metrics/SqlServer/ScalarQuery))
- Network Upload Speed ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/Metrics/NetworkSpeed))
- Network Download Speed ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/Metrics/NetworkSpeed))

**Custom**

- C#/VB.NET ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/Custom/NET))
- PowerShell ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/Custom/PowerShell))
- Batch Script ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/Custom/BatchFile))

Can't find the plugin you were looking for?
Submit a feature request on [GitHub](https://github.com/AnyStatus/Support/issues) or the [Support Portal](https://anystatus.helprace.com/s1-general/ideas).

Need a custom tailor-made plugin? [Contact Us](mailto:info@anystat.us)
