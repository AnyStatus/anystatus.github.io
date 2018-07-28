---
layout: docs
title: Documentation
sub_title: API Reference
---

AnyStatus API is a .NET class library that contains the classes, interfaces and utilities needed for developing AnyStatus extensions and plugins.

### How it works
---------------

AnyStatus automatically loads all widgets and plugins during startup.
Widgets are controlled using interfaces and attributes.
Each widget includes a set of plugable classes that describe its behaviour and characteristics
and handlers that perform the actual work such as retrieving the status.

![AnyStatus Components](/assets/images/AnyStatusComponents.png)

_AnyStatus components_.

### Example
-------------------

The following class is an example for a plugable health check widget.
This class defines the widget properties (name, interval, etc.) and the attributes that are used to control which properties are required
and how the widget is displayed in the user interface.

{% gist c06a60e1f602511ac5f2b43c28582065 %}

Because the Ping class implements IHealthCheck and ISchedulable, AnyStatus will automatically call the following class to perform the health check.

{% gist 1fd5b587b42e358570b99abeaadcf4a3 %}

That's it. No need to register these classes anywhere. AnyStatus will automatically scan and register all plugins during startup and 
the widget will automagically appear in the Add Widget window.

**Want to see more examples?** Check out the open-source plugins library on [GitHub](https://github.com/AnyStatus/Plugins).
