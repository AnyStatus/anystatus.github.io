---
layout: post
title: AnyStatus 3 Preview 1
author: Alon Amsalem
date:   2020-05-09 19:00
tags: [New Releases]
---

I'm pleased to announce the availability of AnyStatus 3 Preview 1 for download on the [Microsoft Store](https://www.microsoft.com/en-us/p/anystatus/9p044vpk62sb). The new version includes various new features, bugs fixes, and improvements. For a detailed list of all changes, please refer to the [Release Notes](/docs/release-notes).

### Release Highlights

##### Endpoints

Endpoints is a new feature that helps users maintain their accounts and connections to their servers more easily. Endpoints are shared across multiple widgets and configurations, to make it easier for users to maintain their dashboard configuration. Examples include, Jenkins, Azure DevOps, Docker, NuGet, SQL Server and more.

##### New User Interface

The user interface has been revamped to provide an easy-to-use interface that boosts user experience. It includes almost all functions available in previous versions plus a number of new features and enhancements. Its highly improved performance allows tens and hundreds of widgets to connect simultaneously. Intuitive dashboard and windows with in-line help guide users in their daily work.

##### Improved API SDK

A newly improved API SDK has been introduced in this release. The new API SDK provides a better fine-grained control over the features and behaviors of widgets.

##### Better Context Menu

The new widgets context-menu experience has been significantly improved and replaced by a new run-time "AI" that renders only the features and options that are explicitly supported by the selected widget on the dashboard. As a result, for example, the user will not be able to remove dynamically added child widgets, such as Jenkins Jobs under a Jenkins View.

##### Separated Configuration Files

In previous releases, the user's information is all encrypted into a single database file. This causes issues for organizations who distribute AnyStatus pre-configured installation for multiple end-users. In the new release, the configuration system is more flexible by using separate JSON configuration files for the application, user preferences, session and dashboard settings. This improvement will hopefully enable more advanced distribution scenarios.
