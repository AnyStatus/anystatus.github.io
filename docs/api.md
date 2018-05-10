---
layout: docs
title: Documentation
sub_title: AnyStatus API
---

AnyStatus API is a .NET class library that contains the classes, interfaces and utilities needed for developing AnyStatus extensions and plugins.

### How it works
---------------

AnyStatus communicates with plugins using the API library. During startup, AnyStatus scans assemblies in the installation directory and registers all plugins.

A plugin is a set of classes that instruct AnyStatus how to display it in the dashboard and which features the plugin supports.

![AnyStatus Components](/assets/images/AnyStatusComponents.png)

_AnyStatus modules_.

### Health Check Example
-------------------

The following class is an example for a plugable health check plugin (widget).
This class contains the widget properties (Name, Interval, etc.) and the attributes that are used to control which properties are required
and how the widget is displayed in the user interface.

{% gist d37e580788eaec8d62858f5bb0cbd246 %}

Because the Ping class implements IHealthCheck and ISchedulable, AnyStatus will automatically call the following class to perform the health check.

{% gist 541ea7571b46f7404818f8c3a8eecf89 %}

That's it. No need to register these classes anywhere. AnyStatus will automatically scan and register all plugins during startup and 
the widget will automagically appear in the Add Widget window.

**Want to see more examples?** Check out the open-source plugins library on [GitHub](https://github.com/AnyStatus/Plugins).
