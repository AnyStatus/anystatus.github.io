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

Endpoints is a new feature that helps users easily maintain their accounts and connections to remote servers and cloud services, such as Jenkins, Azure DevOps (coming soon), Docker, and NuGet. Endpoints can be shared by multiple widgets and configurations, to enable users change credentials or host address in one place, for all widgets in the dashboard.

##### New User Interface

The user interface has been revamped to provide an easy-to-use interface that boosts user experience. It includes almost all functions available in previous versions plus a number of new features and enhancements. Its highly improved performance allows tens and hundreds of widgets to connect simultaneously. Intuitive dashboard and windows with in-line help guide users in their daily work.

##### Improved API SDK

A newly improved API SDK has been introduced in this release. The new API provides better fine-grained control over the features and behaviors of the widgets.

##### Better Context Menu

The new widgets context-menu experience has been significantly improved by a new run-time "AI" that renders only the features and options that are explicitly supported by the selected widget on the dashboard. As a result, for example, the user will not be able to remove dynamically added child widgets, such as Jenkins Jobs under Jenkins View.

##### Separated Configuration Files

In previous releases, the user's information is all encrypted into a single database file. This causes issues for organizations who distribute AnyStatus pre-configured installation for multiple end-users or teams that automatically generated and distribute the team's dashboard configuration. In the new release, the configuration system is now more flexible by using separate JSON configuration files for the application, user preferences, session, endpoints, and dashboard settings. This improvement will hopefully enable more advanced distribution scenarios.
