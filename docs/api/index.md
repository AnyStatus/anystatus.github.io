---
layout: docs
title: AnyStatus API
---

AnyStatus API is a .NET class library that contains the classes, interfaces and utilities needed for developing extensions and plugins for AnyStatus.

### How it works
----------------

A plugin is a set of classes that implement different features. There are classes that implements priodic health checks (such as HTTP health check) or metric queries (such as Weather update or CPU Usage) and there are classes that implements tasks such as Start, Stop and Restart.

AnyStatus scans the installation directory for plugins. It will look for assemblies with a name that starts with "AnyStatus". For example: AnyStatus.Plugins.dll

Other aspects such as the display name, and description are described using attributes.

![AnyStatus Components](/assets/images/AnyStatusComponents.png)

<p></p>

### Widget Example
-------------------

The following class is an example for a plugable health check widget.
This class defines the widget properties (name, interval, etc.) and the attributes that are used to control which properties are required
and how the widget is displayed in the user interface.

{% gist c06a60e1f602511ac5f2b43c28582065 %}

Because the Ping class implements IHealthCheck and ISchedulable, AnyStatus will automatically call the following class to perform the health check.

{% gist 1fd5b587b42e358570b99abeaadcf4a3 %}

That's it. No need to register these classes anywhere. AnyStatus will automatically scan and register all plugins during startup and 
the widget will automagically appear in the Add Widget window.

For more examples, check out the open source plugins library on [GitHub](https://github.com/AnyStatus/Plugins).
