---
layout: docs
title: Documentation
sub_title: API Reference
---

### Widgets
-----------

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

#### Initialize
---------------

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

#### Start
-----------

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
----------

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
------------

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
