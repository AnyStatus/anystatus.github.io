---
layout: docs
title: Documentation
sub_title: API Reference
---

### Tasks

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
