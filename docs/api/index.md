---
layout: docs
title: Documentation
sub_title: AnyStatus API
description: AnyStatus end-user documentation
---

AnyStatus API is a .NET class library that contains the classes, interfaces and utilities needed for developing AnyStatus extensions and plugins.

<br/>

### How it works
---------------

AnyStatus communicates with plugins using the API library. During startup, AnyStatus scans assemblies in the installation directory and registers all plugins.

A plugin is a set of classes that instruct AnyStatus how to display it in the dashboard and which features the plugin supports.

<br/>

![AnyStatus Components](/assets/images/AnyStatusComponents.png)

<br/>

### Plugin Example
------------

A class that defines the widget and its properties.

```csharp
[DisplayName("Ping")]
[DisplayColumn("Network")]
[Description("Test the reachability of a host.")]
public class Ping : Widget, IHealthCheck, ISchedulable
{
    [Category("Ping")]
    [Description("Host Name or IP Address")]
    public string Host { get; set; }
}
```

A class that performs the widget health check.

```csharp
public class Pong : ICheckHealth<Ping>
{
    public async Task Handle(HealthCheckRequest<Ping> request, CancellationToken cancellationToken)
    {
        using (var pinger = new System.Net.NetworkInformation.Ping())
        {
            var reply = await ping.SendPingAsync(request.DataContext.Host);

            request.DataContext.State = (reply.Status == IPStatus.Success) ? State.Ok : State.Failed;
        }
    }
}
```

That's it. No need to register these classes anywhere. AnyStatus will scan and register all plugins during startup.
The widget will automagically appear in the Add Widget window with all of its properties.


**Want to see more examples?** Check out the open-source plugins library on [GitHub](https://github.com/AnyStatus/Plugins).
