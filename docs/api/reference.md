---
layout: docs
title: Documentation
sub_title: API Reference
---

### Health Check
----------------

```
public class MyHealthCheck : Widget, IHealthCheck
{
}
```

```
public class MyHealthChecker : ICheckHealth<MyHealthCheck>
{
    public async Task Handle(HealthCheckRequest<MyHealthCheck> request, CancellationToken cancellationToken)
    {
    }
}
```