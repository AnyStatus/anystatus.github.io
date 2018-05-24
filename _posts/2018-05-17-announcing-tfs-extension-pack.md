---
layout: post
title: Announcing TFS Extension Pack
author: Alon Amsalem
date:   2018-05-27 11:30
tags: [TFS, VSTS]
---

I'm pleased to announce the initial release of TFS Extension Pack for AnyStatus, now available at [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=anystatus.TFSExtensionPack).

This is an early release which requires [AnyStatus extension for Visual Studio](https://marketplace.visualstudio.com/items?itemName=AlonAmsalem.AnyStatus) version 2.1 or above to be installed.

The new extension pack installs additional premium widgets in AnyStatus for TFS (and VSTS) builds, releases and work items.

The extension pack is free for the beta period until September 1, 2018. After that, a perpetual license will be required.

There are two main reasons why I chose to separate the widgets to another extension;
First, to let users choose whether or not to install the additional .NET client libraries needed.
Secondly, I was looking for a way to monetize AnyStatus without polluting the user expirience or giving up the free version.
By doing so, I believe it will help AnyStatus last longer and grow wider.

Hopefully, additional extension packs for Jenkins, SonarQube, Octopus Deploy and others will be released further down the road.

**Please note** TFS extension pack is a work in progress, the actions have not been implemented yet, only basic functionality at this point. If you experience any issues or would like to suggest changes, please [contact us](/support).

**Also note** to open a settings file that contains references to the widgets in the TFS Extension Pack, the TFS Extension Pack must be installed. Otherwise, the settings file will not load.

If you have any questions, let me know in the comments section below or via the [support channels](/support).

Thank you for using AnyStatus!
