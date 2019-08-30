---
layout: post
title: Count Processes And Threads
redirect_from: "/2019/02/17/view-processes-and-threads.html"
author: Alon Amsalem
date:   2019-02-17 12:00
tags: [Performance Counters]
---

Performance counters are used to provide information as to how well the operating system or an application is performing. The performance counter data can help determine system bottlenecks and fine-tune system and application performance. Using AnyStatus it is easy to view performance counters such as the number of processes and threads running on your system.

## Performance Counter Widget

Add a new widget using the dashboard context menu or the + icon in the main menu. In the "Add Widget" window select **Performance Counter** under **Metrics** category.

Type *System* in the Categy field and in the Counter field type *Processes* or *Threads*.
Enter a name for the widget in the Name field and click **Add** to save the widget in the dashboard.

![AnyStatus Desktop 2.4.1](/assets/posts/2019-02-17-view-processes-and-threads/add-performance-counter-widget.png)

The performance counter data will update immediately. After a couple of refreshes, a sparkline chart will apear on the right side of the performance counter widget.
You can set the color of the chart in the widget properties window.

![AnyStatus Desktop 2.4.1](/assets/images/screenshots/anystatus_desktop_2.4.1.png)

Feel free to suggest other interesting and useful performance counters in the comments section below.