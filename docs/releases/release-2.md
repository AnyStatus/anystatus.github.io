---
layout: docs
title: Release Notes
---

### Release 2.9
------------------
<p class="text-muted">2019-10-21</p>

Features

- [#109](https://github.com/AnyStatus/Support/issues/109) Start AnyStatus minimized when Windows starts
- [#35](https://github.com/AnyStatus/Support/issues/35) NuGet Package Widget

### Release 2.8
------------------
<p class="text-muted">2019-09-06</p>

Features

- [#160](https://github.com/AnyStatus/Support/issues/160) Elasticsearch plugins by Fatih Boy.
- [#161](https://github.com/AnyStatus/Support/issues/161) Redis plugins by Fatih Boy.
- [#170](https://github.com/AnyStatus/Support/issues/170) Kubernetes plugins by Fatih Boy.

Bug Fixes

- [#169](https://github.com/AnyStatus/Support/issues/169) Fixed parent widgets folder summary alignment.

### Release 2.7
------------------
<p class="text-muted">2019-08-28</p>

Features

- Azure DevOps plugins are now shipped out-of-the-box. Please uninstall Azure DevOps Plugins installation before installing AnyStatus v2.7
  - New Widgets
    - Pull Requests Widget.
    - Work Items Query Widget.
- Logical Drive Usage widget.
- Active TCP Connections widget.

- Added a link to Feedback page from left menu.
- [#165](https://github.com/AnyStatus/Support/issues/165) Configuration settings encryption is now optional. You can now enable or disable encryption in the settings window. Encryption is enabled by default.

Bug Fixes

- [#153](https://github.com/AnyStatus/Support/issues/153) Display correct temperature values on non-english machines in Weather widget.
- [#158](https://github.com/AnyStatus/Support/issues/158) Sparkline chart does not re-scale.
- Fixed left menu background color in Light Theme.

Changes

- Added sparkline chart to Upload and Download widgets.
- Use default widget name when adding new widgets.
- Minor user interface changes.
  - Changed Add Widget toolbar icon.
  - Removed window border.
  - Changed widgets background and mouse-over colors.
  - Changed toolbar and left menu colors.
- Removed success messages when importing and exporting settings.
- Renamed _Ok_ button to _Save_ in Settings window.
- Renamed Options to Settings in various places.

API Changes

- "Symbol" property of [Metric](https://github.com/AnyStatus/API/blob/master/src/AnyStatus.API/Widgets/Types/Metric.cs) is now obsolete.

### Release 2.6.13
------------------
<p class="text-muted">2019-06-14</p>

Bug Fixes

- [#147](https://github.com/AnyStatus/Support/issues/147) Window size and location not saved when exiting from system tray.

Improvements

- Added vertical scrolling to left menu.

### Release 2.6.10
------------------
<p class="text-muted">2019-06-11</p>

Features

- [#141](https://github.com/AnyStatus/Support/issues/141) System Information widgets category.
- [#142](https://github.com/AnyStatus/Support/issues/142) GitHub Repository Issues widget.
- [#134](https://github.com/AnyStatus/Support/issues/134) RAM Usage widget.
- [#123](https://github.com/AnyStatus/Support/issues/123) Process CPU Usage widget.
- [#138](https://github.com/AnyStatus/Support/issues/138) Page File Usage widget.
- [#135](https://github.com/AnyStatus/Support/issues/135) Process Count widget.
- [#136](https://github.com/AnyStatus/Support/issues/136) Thread Count widget.

Changes

- Minor UI changes in Options window.

Credits

- Special thanks to [Toby Smith](https://tobysmith.uk/) for contributing several plugins and bug fixes in recent releases.

### Release 2.5.22
------------------
<p class="text-muted">2019-05-26</p>

Bug Fixes

- [#126](https://github.com/AnyStatus/Support/issues/126) Window always opens in dark theme.
- [#125](https://github.com/AnyStatus/Support/issues/125) Window always docks to primary window.
- [#122](https://github.com/AnyStatus/Support/issues/122) Window is off screen when disconnecting extended monitor.
- [#121](https://github.com/AnyStatus/Support/issues/121) Stuck sub-pixel in application icon.

Changes

- Removed "Show debug information in the output window".

### Release 2.5
---------------
<p class="text-muted">2019-05-06</p>

Features

- New User Interface. [Read more](/2019/04/20/introducing-the-new-user-interface.html).
- [#120](https://github.com/AnyStatus/Support/issues/120) Battery Meter Widget.
- Added read-only Priority column to Color Theme table in settings window.
- Allow metrics to have child nodes.

Changes

- Code signing certificate has been renewed.
- Removed minimize button from all windows.
- Auto-size dialog boxes to fit content.
- Options has been renamed to Settings.
- Widgets can now replace the default tooltip text with custom text.
- Slightly darker window background.
- Trim long widget names instead of horizontal scrolling.
- Added [RestSharp](http://restsharp.org/) for plugins who use REST calls.

Bug Fixes

- No confirmation dialog when restoring default color theme.

System Requirements

- Microsoft .NET Framework 4.6.2 or above.
- Added Visual Studio 2019 support.

API

- Allow widget handlers to invoke other widget handlers to support use-cases such as refreshing a build status before starting a new build.
- New [IUiAction](https://github.com/AnyStatus/API/blob/95c893b46aed748218d309243ebe93f88d8bb04c/src/AnyStatus.API/Common/Services/IUIAction.cs) interface for invoking actions on UI thread.

### Release 2.4
--------------------
<p class="text-muted">2019-02-16</p>

Changes

- Themed dialog windows in AnyStatus Desktop.
- Folders such as Azure DevOps (VSTS) Release and Jenkins View are now collapsed by default.
- Changed "Units" to "Interval Units" in widget properties window.
- Hide interval-units when editing folders.
- Changed widget category "Code" to "Custom".
- Moved "Options" from context menu to main menu.
- Changed default interval of performance counters to 30 seconds.
- Changed default sparkline colore to green.
- Changed window close and minimized button colors in light theme.
- Shorten text for widgets with very long name to prevent horizonal scrolling.
- Trim whitespace from tooltips.

Bug Fixes

- [#104](https://github.com/AnyStatus/Support/issues/104) Bug: VSTS build names with special characters fail.
- [#112](https://github.com/AnyStatus/Support/issues/112) Bug: Folder name is not saved when clicking on window background while editing folder name.

Breaking Changes

- TFS extension pack has been retired and replaced with Azure DevOps Plugins.
- Minor API changes.

### Release 2.3.26
------------------
<p class="text-muted">2018-11-21</p>

Changes

- Added sparkline to Performance Counter widget.
- Round metric value.

### Release 2.3
------------------
<p class="text-muted">2018-08-26</p>

Features

- Light and Dark themes for AnyStatus Desktop (beta).
- API support for sparklines (line chart).
- Added a sparkline to CPU Usage widget.
- Allow user to specify interval units of seconds or minutes (default).
- VSTS Releases: Use "All Tasks -> Start" to create a new release.
- VSTS Release Environment: Use "All Tasks -> Start" to deploy latest release to selected environment.

Bug Fixes

- Fixed a bug in root context menu after selecting a widget.
- Hide error dialog when checking for updates fail.

Improvements

- Show "pause" icon when a metric widget is disabled.
- Minor UI improvements.

Changes

- When refreshing, write a single line to the activity log instead of one for each widget that is being refreshed.

### Release 2.2
------------------
<p class="text-muted">2018-08-16</p>

Features

- [#85](https://github.com/AnyStatus/Support/issues/85) Trigger scripts, executables and custom notifications on any status change.
- [#44](https://github.com/AnyStatus/Support/issues/44) Use Alt+Up and Alt+Down to move widgets.
- Auto-download AnyStatus updates when a new version is available.
  - Include pre-release versions when checking for updates.

Bug Fixes

- [#99](https://github.com/AnyStatus/Support/issues/99) Performance Counter widget fails due to "The network path was not found".

Changes

- TeamCity build: hide user name and password when "Use guest user" is checked.
- Jenkins job: hide parameters when "Parameterized Build" is unchecked.
- Categories in "Add Widget" window have changed to DevOps, Health Checks, Metrics and Other.

Improvements

- Minor UI performance improvements.

### Release 2.1.23
------------------
<p class="text-muted">2018-06-16</p>

Features

- [#64](https://github.com/AnyStatus/Support/issues/64) Persist AnyStatus Desktop window size, position and docking.

### Release 2.1.18
------------------
<p class="text-muted">2018-06-15</p>

Features

- [#91](https://github.com/AnyStatus/Support/issues/91) Enable customizing status icons via Color Theme tab in Options window.

Bug Fixes

- [#90](https://github.com/AnyStatus/Support/issues/90) AnyStatus Desktop window disapears when docked in high DPI displays.

Improvements

- Changed the default status color of statuses: Unknown, Canceled, Disabled and None.
- Show an empty circle when status is "None". Reset or edit your Theme in the Options window, to use the new icon.
- Disable "All Tasks" when no tasks are available.

### Release 2.1.12
------------------
<p class="text-muted">2018-05-30</p>

Improvements

- [#88](https://github.com/AnyStatus/Support/issues/88) Changed the order of items in the context menu and moved tasks such as Start, Stop, Restart in to "All Tasks" group. [Read more](https://github.com/AnyStatus/Support/issues/88)

### Release 2.1.9
----------------
<p class="text-muted">2018-05-25</p>

Bug Fixes

- Fixed Jenkins Job progress indicator.

### Release 2.1
----------------
<p class="text-muted">2018-05-16</p>

Features

- AnyStatus extension packs support.
- TFS extension pack (currently available for Visual Studio only).
- Open AnyStatus extension from Tools menu in Visual Studio.
- Job History (histogram) support - widgets can now show recent history of jobs such as builds, releases, etc.
- Added "Open" and "Save As" buttons to AnyStatus Desktop toolbar.
- Added more options to the system tray icon of AnyStatus Desktop.
- Allow pasting widgets on the dashboard.

Improvements

- Simplified error messages.
- Improved VSTS Release status.
- Minor UI changes and improvements.

Bug Fixes

- Fixed a bug when closing Activity Log window in AnyStatus Desktop.
- Fixed a bug when clicking on the tray icon to show or hide AnyStatus Desktop.
- Fixed a bug when minimizing AnyStatus Desktop window.

### Release 2.0.62
------------------
<p class="text-muted">2018-04-18</p>

Bug Fixes

- [#83](https://github.com/AnyStatus/Support/issues/83) Fixed "Open in Browser" of various widgets, including VSTS. Thanks to Patrick Kalkman.

Changes

- [#82](https://github.com/AnyStatus/Support/issues/82) Moved Port health check widget to Network category.

### Release 2.0.57
------------------
<p class="text-muted">2018-03-29</p>

Bug Fixes

- Fixed VSTS build widget.

### Release 2.0.55
------------------
<p class="text-muted">2018-03-23</p>

Improvements

- AnyStatus API 2.0
- Improved overall performance, stability and memory utilization.
- Changed dependency injection framework to SimpleInjector.
- Changed AnyStatus custom mediator with MediatR.

Changes

- Dashboard UI tree-view node fills more space.
- Several activity log messages text has changed.

System Requirements

- Microsoft .NET Framework 4.6 or above
