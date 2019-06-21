---
layout: docs
title: API Documentation
---

AnyStatus API is a .NET class library that contains the classes, interfaces and utilities needed for developing extensions and plugins for AnyStatus.

### How It Works

AnyStatus scans the installation directory for plugins in assemblies who's name start with "AnyStatus". For example: AnyStatus.Plugins.dll

A plugin consists of a single Widget class and multiple classes that implement each feature separately. These include, health check, metric query, start, stop, restart, open web page, validation, notifications, triggers and more.

Other aspects such as the display name, and description are described using attributes.

![AnyStatus Components](/assets/images/AnyStatusComponents.png)

<p></p>

### Examples

The following class is an example for a plugable health check widget.
This class defines the widget properties (name, interval, etc.) and the attributes that are used to control which properties are required
and how the widget is displayed in the user interface.

{% gist c06a60e1f602511ac5f2b43c28582065 %}

Because the Ping class implements IHealthCheck and ISchedulable, AnyStatus will automatically call the following class to perform the health check.

{% gist 1fd5b587b42e358570b99abeaadcf4a3 %}

That's it. No need to register these classes anywhere. AnyStatus will automatically scan and register all plugins during startup and 
the widget will automatically appear in the Add Widget window.

For more examples, check out the open source plugins library on [GitHub](https://github.com/AnyStatus/Plugins).
