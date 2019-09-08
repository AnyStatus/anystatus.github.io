---
layout: post
title: AnyStatus Release 2.8
author: Alon Amsalem
date:   2019-09-07 16:00
tags: [New Releases]
---

AnyStatus 2.8 has been released! The latest release includes new widgets, bug fixes and UI changes. Download is available from our [Website](https://www.anystat.us/downloads), [Microsoft Store](https://www.microsoft.com/en-us/p/anystatus/9p044vpk62sb), and [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=anystatus.AnyStatus).

## What's New

AnyStatus 2.8 adds 32 new powerful open-source widgets for [Elasticsearch](https://www.elastic.co/), [Redis](https://redis.io/), and [Kubernetes](https://kubernetes.io/), developed and maintained by [Fatih Boy](https://github.com/fatihboy/).
You can find more information, including their GitHub repositories, in the links below.
Also, widgets categories have changed. The DevOps category has been canceled, instead, there are separate categories for each service such as AppVeyor, Jenkins, etc. And, Jenkins widgets have been migrated to a new [NuGet package](https://www.nuget.org/packages/AnyStatus.Plugins.Jenkins) and [GitHub repository](https://github.com/AnyStatus/Jenkins).

[#160](https://github.com/AnyStatus/Support/issues/160) Elasticsearch Widgets

- Store Size
- Index Health
- RAM Usage
- Index Store Size
- Index Count
- Index Deleted Document Count
- Cluster Document Count
- Deleted Document Count
- Cluster Health
- File System Usage
- CPU Usage
- Index Document Count

[#161](https://github.com/AnyStatus/Support/issues/161) Redis Widgets

- Total Commands Processed
- Keyspace Key Count
- Used Memory
- Total Connections Received
- Client Count
- Database Count
- Database Size
- Keyspace Expires Count
- Rejected Connections
- Keyspaces Misses
- Blocked Clients
- Used Resident Set Size
- Operations Per Second
- Evicted Keys

[#170](https://github.com/AnyStatus/Support/issues/170) Kubernetes Widgets

- Namespace Count
- Node RAM Usage
- Node CPU Usage
- Pod Count
- Pod RAM Usage
- Pod CPU Usage

## Bug Fixes

- [#169](https://github.com/AnyStatus/Support/issues/169) Fixed misaligned status summary on parent widgets.

## Download

- Downloads: https://www.anystat.us/downloads
- Microsoft Store: https://www.microsoft.com/en-us/p/anystatus/9p044vpk62sb
- Visual Studio Marketplace: https://marketplace.visualstudio.com/items?itemName=anystatus.AnyStatus

## Summary

That's it for this release. Special thanks to Fatih Boy for investing significant time and efforts in this release.
Feel free to leave a comment and let us know what you think.
