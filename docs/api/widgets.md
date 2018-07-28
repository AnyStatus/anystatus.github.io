---
layout: docs
title: Documentation
sub_title: API Reference / Widgets
---

- [Health Check](#health-check)
- [Metric](#metric)
- [Folder](#folder)
- [Build](#build)

#### Health Check
-----------------
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
-----------
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

#### Folder
-----------
```
public class MyFolder : Folder
{
}
```
See [default folder](https://github.com/AnyStatus/API/blob/3f24e47c95c573e5202cc7034c2471a82f11d8eb/src/AnyStatus.API/Widgets/Types/Folder.cs).

#### Build
----------
```
public class MyBuild : Build
{
}
```
See [default build](https://github.com/AnyStatus/API/blob/3f24e47c95c573e5202cc7034c2471a82f11d8eb/src/AnyStatus.API/Widgets/Types/Build.cs).
