---
layout: docs
title: AnyStatus Plugins
---

AnyStatus is an extensible Windows application that rolls up metrics and events from various sources into one simple dashboard. Examples include builds and releases, health checks for different services and operating system metrics.
Check out the [API Documentation](/docs/api) to learn more about AnyStatus extensions and plugins.

## Azure DevOps Plugins

View and control the status of your builds, releases, deployment environments and work items on [Azure DevOps Services](https://azure.microsoft.com/en-us/services/devops/). The Azure DevOps extension pack is a separate installation that adds new widgets with additional features that are not available in the open-source widgets. These include, history, progress, estimated time remaining, custom work item queries, and more. The extension pack is free for the preview period.

For more information and inquiry please [contact us](mailto:info@anystat.us).

<p>
    <form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_top">
        <button class="btn btn-warning" onclick="ga('send', 'event', 'Buy', 'Azure DevOps');">Buy Now</button> 
        <input type="hidden" name="cmd" value="_s-xclick">
        <input type="hidden" name="hosted_button_id" value="DSSVLGELMML32">
        <img alt="Buy Now" src="https://www.paypalobjects.com/en_US/i/scr/pixel.gif" width="1" height="1">
    </form>
    <p class="mt-2"><small class="text-muted">* Usage is free for the preview period.</small></p>
</p>

## Open Source Plugins

These are the default pre-installed widgets that comes free with AnyStatus. The source code is open for modifications and available on [GitHub](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/DevOps/TFS/Build). C# developers are invited to make changes and submit pull requests to help us maintain a free and open source set of tools for everyone to use.

<p class="lead">DevOps</p>

- TFS Build ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/DevOps/Microsoft/TFS/Build))
- Azure DevOps Build ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/DevOps/Microsoft/VSTS/Build))
- Azure DevOps Release ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/DevOps/Microsoft/VSTS/Release))
- Jenkins Job ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/DevOps/Jenkins/Job))
- Jenkins View ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/DevOps/Jenkins/View))
- AppVeyor Build ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/DevOps/AppVeyor/Build))
- TeamCity Build ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/DevOps/TeamCity/Build))
- Coveralls Code Coverage ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/DevOps/Coveralls))

<p class="lead">Health Checks</p>

- Windows Service ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/HealthChecks/WindowsService))
- HTTP/S ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/HealthChecks/HTTP))
- TCP/UDP ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/HealthChecks/PortCheck))
- Ping ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/HealthChecks/Ping))
- SQL Server Connection ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/HealthChecks/SqlServer/Connection))
- IIS Application Pool ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/HealthChecks/IIS/AppPool))
- Uptime Robot ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/HealthChecks/UptimeRobot))
- Pingdom ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/HealthChecks/Pingdom))

<p class="lead">Metrics</p>

- SQL Server Scalar Query ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/Metrics/SqlServer/ScalarQuery))
- Current Weather (Experimental)

<p class="lead">Custom</p>

- C#/VB.NET ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/Custom/NET))
- PowerShell ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/Custom/PowerShell))
- Batch Script ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/Custom/BatchFile))

<p class="lead">System Information</p>

- Battery ([Source](https://github.com/AnyStatus/Plugins/blob/master/src/AnyStatus.Plugins/Widgets/Metrics/Battery/BatteryStatusQuery.cs))
- CPU Usage ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/Metrics/CPU/Usage))
- Performance Counter ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/Metrics/PerformanceCounters))
- Network Upload Speed ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/Metrics/NetworkSpeed))
- Network Download Speed ([Source](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/Metrics/NetworkSpeed))
- Process CPU Usage
- RAM Usage
- Page File Usage
- Process Count
- Thread Count
- Logical Drive Usage
- Active TCP Connections

<p class="lead">Can't find the plugin you were looking for?</p>

Submit a feature request on [GitHub](https://github.com/AnyStatus/Support/issues) or the [Support Portal](https://anystatus.helprace.com/s1-general/ideas).

<p class="lead">Need custom tailor-made plugins?</p>

You can develop and use your own plugins or you can [contact us](mailto:info@anystat.us) to build it for you.
