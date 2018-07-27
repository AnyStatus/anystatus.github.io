---
layout: docs
title: Documentation
sub_title: API Reference
---

### Widgets
-----------

#### Health Check

```
public class MyWidget : Widget, IHealthCheck
{
}
```

```
public class HealthCheckMyWidget : ICheckHealth<MyWidget>
{
}
```

#### Metric

```
public class MyMetric : MetricValue
{
}
```

```
public class MyMetricQuery : IMetricQuery<MyMetric>
{
}
```

### Automation
---------------

#### Scheduler

```
public class MyWidget : Widget, ISchedulable
{
}
```

#### Initialize

```
public class MyWidget : Widget, IInitializable
{
}
```

```
public class InitializeMyWidget : IInitialize<MyWidget>
{
}
```

### Tasks
---------

#### Start

```
public class MyWidget : Widget, IStartable
{
}
```

```
public class StartMyWidget : IStart<MyWidget>
{
}
```

#### Stop

```
public class MyWidget : Widget, IStoppable
{
}
```

```
public class StopMyWidget : IStop<MyWidget>
{
}
```

#### Restart

```
public class MyWidget : Widget, IRestartable
{
}
```

```
public class RestartMyWidget : IRestart<MyWidget>
{
}
```

#### Open in Browser

```
public class MyWidget : Widget, IWebPage
{
	public string URL { get; } => "https://your-web-page";
}
```

```
public class OpenMyWidgetWebPage : IOpenWebPage<MyWidget>
{
}
```
See [default handler](https://github.com/AnyStatus/API/blob/master/src/AnyStatus.API/Widgets/Features/OpenWebPage.cs).