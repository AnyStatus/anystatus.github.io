---
layout: docs
title: AnyStatus Plugins
---

AnyStatus is lightweight desktop application for Windows that brings together metrics and events from various sources.
Examples include CI/CD pipelines, health checks, operating system metrics, network, servers, databases and more.

To learn more about developing plugins for AnyStatus, please refer to the [API Documentation](/docs/api).

## Plugins

These are the default pre-installed widgets that comes free with AnyStatus. The source code is open for modifications and available on [GitHub](https://github.com/AnyStatus/Plugins/tree/master/src/AnyStatus.Plugins/Widgets/DevOps/TFS/Build). C# developers are invited to make changes and submit pull requests to help us maintain a free and open source set of tools for everyone to use.

### Azure DevOps

- Build
- Release
    - Deployment Environment
- Work Items
- Pull Requests

### Team Foundation Server

- Build

### Jenkins

- Job
- View

### TeamCity

- Build

### AppVeyor

- Build

### Custom

- C#/VB.NET Script
- PowerShell
- Batch Script

### GitHub

- Issues

### NuGet

- NuGet Package

### SQL Server

- Connection
- Scalar Query

### Health Checks

- HTTP/S
- Windows Service
- Ping
- TCP/IP Port
- IIS Application Pool
- Uptime Robot
- Pingdom

### System Information

- Performance Counter
- Battery
- CPU Usage
- Process CPU Usage
- RAM Usage
- Process RAM Usage
- Logical Drive Usage
- Page File Usage
- Process Count
- Thread Count
- Folder Exists
- File Exists
- Network Upload/Download Speed
- Active TCP Connections

### Other

- Coveralls Code Coverage
- Current Weather

## Can't find the plugin you were looking for?

Submit a feature request on [GitHub](https://github.com/AnyStatus/Support/issues) or the [Support Portal](https://anystatus.helprace.com/s1-general/ideas).

## Need custom tailor-made plugins?

You can develop and use your own plugins or you can [contact us](mailto:info@anystat.us) to build it for you.
