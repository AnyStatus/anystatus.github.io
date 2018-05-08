---
layout: post
title:  AnyStatus plugins are now open source!
date:   2017-06-22 10:00:00
author: AlonAm
redirect_from: "/2017/06/22/all-plugins-are-now-open-source.html"
---

This week, I have separated all plugins from the main code base and moved them to a new open-source project to enable developers improve or add new plugins to the growing library.

To support the plugins library, I have created a new API library, which contains all the classes, interfaces and other utilities needed to develop plugins for AnyStatus.

Both libraries are hosted on [GitHub](https://github.com/anystatus) and published to [NuGet](https://www.nuget.org/packages?q=anystatus) using [AppVeyor](https://ci.appveyor.com/project/AnyStatus/plugins).
Developers are invited to create pull requests, suggest new ideas, report bugs and contribute to the documentation.

## How it works
---------------

<div class="row">
  <div class="col-md-9">
<p>AnyStatus communicates with plugins using the API library. During startup, AnyStatus scans assemblies in the installation directory and registers all plugins.</p>

<p>A plugin is a set of classes that instruct AnyStatus how to display it in the dashboard and how to handle custom actions such as monitoring and triggering builds.</p>

<p>Plugins can be decorated with attributes such as DisplayName, Category and Description.</p>
  </div>
  <div class="col-md-3">
    <img src="/assets/posts/2017-06-22-all-plugins-are-now-open-source/plugins-flow-chart.png"/>
  </div>
</div>

<br/>

### Plugin Example
------------------

A class that defines the plugin.

{% gist d37e580788eaec8d62858f5bb0cbd246 %}

A class that handles monitor health checks.

{% gist 541ea7571b46f7404818f8c3a8eecf89 %}
