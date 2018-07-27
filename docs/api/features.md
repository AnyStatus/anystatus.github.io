---
layout: docs
title: Documentation
sub_title: API Reference
---

### Features

<br/>

##### Job Scheduler

```
public class MyWidget : Widget, ISchedulable
{
}
```

##### Progress Bar

```
public class MyWidget : Widget, IReportProgress
{
}
```

##### Histogram

```
public class MyWidget : Widget, IJobHistory
{
}
```

##### Initialize

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

##### Open in Browser

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
