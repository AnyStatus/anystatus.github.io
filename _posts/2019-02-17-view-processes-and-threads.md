---
layout: post
title: Using AnyStatus to view processes and threads
author: Alon Amsalem
date:   2019-02-17 12:00
tags: [Performance Counters]
---

Performance counters are used to provide information as to how well the operating system or an application is performing. The performance counter data can help determine system bottlenecks and fine-tune system and application performance. Using AnyStatus it is easy to view performance counters such as the number of processes and threads running on your system.

### Step 1: Add a new widget

Add a new widget using the dashboard context menu or the + icon and select **Performance Counter** under **Metrics** category.
In the Category field type *System* and in the Counter field type *Processes* or *Threads*.
Enter a name for the widget in the Name field.

![AnyStatus Desktop 2.4.1](/assets/posts/2019-02-17-view-processes-and-threads/add-performance-counter-widget.png)

### Step 2: Save

Click **Test** to test the widget before saving and then **Add** to save the widget in the dashboard.
After a couple of refreshes, a sparkline chart will apear next to the performance counter widget.
You can change the color of the chart in the widget properties under Sparkline section.

![AnyStatus Desktop 2.4.1](/assets/images/screenshots/anystatus_desktop_2.4.1.png)

Feel free to suggest other interesting and useful performance counters in the comments section below.