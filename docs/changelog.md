---
layout: docs
title: Documentation
sub_title: Changelog
redirect_from: "changelog"
---

These are the changes to each version that has been released on our website and the official [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=AlonAmsalem.AnyStatus).


### Release 2.3.X
------------------
<p class="text-muted">Coming soon...</p>

Bug Fixes

- Enable special characters in build definition name in VSTS and TFS widgets.

Changes

- Dark and light themed dialog windows.

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

[Read more](/2018/03/23/AnyStatus-Release-2.0-Alpha.html)

### Release 1.6.7
-----------------
<p class="text-muted">2018-03-18</p>

Bug Fixes

- Fixed a bug when resizing and then docking AnyStatus Desktop window.

### Release 1.6.4
-----------------
<p class="text-muted">2018-03-06</p>

Bug Fixes

- [#80](https://github.com/AnyStatus/Support/issues/60) Fixed a copy-paste bug.
- [#60](https://github.com/AnyStatus/Support/issues/60) Redundant Jenkins jobs in Jenkins view widget.

### Release 1.6.2
-----------------
<p class="text-muted">2018-02-25</p>

Features

- [#9](https://github.com/AnyStatus/Support/issues/9) Copy and Paste dashboard widgets.
- [#65](https://github.com/AnyStatus/Support/issues/65) Added *Enable All* and *Disable All* buttons to the dashboard context menu.

Improvements

- Slightly faster startup.
- More unit and integration tests.

Changes

- Removed help button from Visual Studio extension toolbar. Help and support information is available in the Options window.

### Release 1.5.32
-----------------
<p class="text-muted">2018-02-20</p>

Features

- [#72](https://github.com/AnyStatus/Support/issues/72) Run AnyStatus Desktop when Windows starts.

Bug Fixes

- Fixed a bug in activity log context menu.


### Release 1.5.29
-----------------
<p class="text-muted">2018-02-18</p>

Features

- [#42](https://github.com/AnyStatus/Support/issues/42) Copy rows from activity log to clipboard in AnyStatus Desktop.


### Release 1.5.24
-----------------
<p class="text-muted">2018-02-11</p>

Features

- HTTP/S - Option to use default credentials. Thanks to Nietha.
- AppVeyor - Optionally trigger specific branch. Thanks to Matt McKinstry.


### Release 1.5.21
-----------------
<p class="text-muted">2017-12-22</p>

Features

- [#59](https://github.com/AnyStatus/Support/issues/59) Dock dashboard window to the side of the screen in AnyStatus Desktop
- Auto-hide dashboard when window is docked in AnyStatus Desktop.
- Added an option to show or hide desktop notifications when errors occur and recover. By default, all widgets will show error notifications except builds. To reduce the number of notifications during network failures.
- Added help tab to options page in AnyStatus for Visual Studio.

Changes

- Removed Help button from main menu in AnyStatus Desktop.
- Replaced About page with Help page.

Bug Fixes

- [#61](https://github.com/AnyStatus/Support/issues/61) Don't report build failure if network has problem 


### Release 1.4.101
-----------------
<p class="text-muted">2017-11-03</p>

This release includes an update for TeamCity builds thanks to [Shmueli Englard](https://twitter.com/Shmuelie) and other minor changes.

Features

- Added support for branches in TeamCity builds. You can now monitor builds of specific branches.
- Added more information to TeamCity build failed notification.

Changes

- API Token is no longer required for AppVeyor builds. You can now monitor any public AppVeyor build.
- Visual Studio package manifest.
- Increased properties window size.


### Release 1.4.96
-----------------
<p class="text-muted">2017-10-31</p>

Features

- Trigger VSTS Build.
- Open VSTS Build in browser.
- Open VSTS Release in browser.

Improvements

- Context menu actions such as, trigger a build, will be disabled when the status is None or Error.
- Improved build notifications text and behaviour - will not show notifications when the status change from Error to Ok.
- Disable "check for updates" feature when running as UWP.


### Release 1.4.87
-----------------
<p class="text-muted">2017-10-23</p>

Bug Fixes

- Fixed build status issue in VSTS Build plugin (preview).
- Fixed tooltip text of Jenkins Job plugin when job is running.

Improvements

- Larger status icons
- Changed import/export success messages.


### Release 1.4.66
-----------------
<p class="text-muted">2017-09-22</p>

Features

- VSTS Build Plugin (Preview).

Improvements

- Added "Parameterized Build" property to Jenkins Job plugin - the default behaviour has changed.
- Added support for [personal access tokens](https://docs.microsoft.com/en-us/vsts/accounts/use-personal-access-tokens-to-authenticate) in VSTS plugins.
- Improved help text in VSTS plugins.


### Release 1.4.63
-----------------
<p class="text-muted">2017-09-21</p>

Features

- VSTS Release Plugin (Preview).
- Jenkins View Plugin by Alexander Kolky (Preview).
- Added test button to properties window.
- Press F5 to refresh the entire tree or selected node in AnyStatus Desktop.
- Added a link to downloads page when a new version is available in AnyStatus Desktop.

Improvements

- Added support for plugins to add/remove other plugins at runtime.
- Added lots of unit tests, integration tests and automated UI tests.
- Added icons to context menus in AnyStatus Desktop.
- Dynamically generated context menus.
- Jenkins plugins refactoring.
- Added CSRF protection support to Jenkins Job plugin.
- Improved general options UI.
- Highlight tree node on mouseover.
- Changed tree nodes size, colors, margin and cursor.
- Added success message to restore defaults command.
- Removed Visual Studio dependencies from core project.
- Added window shadow and border to AnyStatus Desktop.
- Added version number at the bottom of the main window in AnyStatus Desktop.
- Custom scrollbar colors in AnyStatus Desktop.

Bug Fixes

- [#33](https://github.com/AnyStatus/Support/issues/33) Trigger new build for Jenkins throws an exception.
- [#32](https://github.com/AnyStatus/Support/issues/32) Left mouse click on background doesn't unselect node.
- [#31](https://github.com/AnyStatus/Support/issues/31) Drag and drop issue.
- [#26](https://github.com/AnyStatus/Support/issues/26) Context menus not opening in some areas in AnyStatus Desktop.
- [#25](https://github.com/AnyStatus/Support/issues/25) Notifications tray icon remains after closing.
- Fixed expand/collapse issue in AnyStatus Desktop.
- Fixed a bug when tree nodes are clicked but not selected.


### Release 1.3.45
-----------------
<p class="text-muted">2017-08-22</p>

Bug Fixes

- Fixed [issue 22](https://github.com/AnyStatus/Support/issues/22): When creating two items of the same type, the second item overwrites the first one.


### Release 1.3.44
------------------
<p class="text-muted">2017-07-02</p>

Features

- SQL Scalar Query - Show the return value of a scalar SQL query in the dashboard.
- Check for new updates at startup. New version details is shown in the activity log.
- Show success message after restoring default settings.
- Use interval 0 to bypass monitors. Monitor check will run once and when refreshing the status.

Changes

- Open source AnyStatus API library.
- Open source AnyStatus Plugins library.
- Changed notification messages text.

Improvements

- Removed unused assembly references to reduce package size.
- Cleaner "Add new item" user interface.
- Show one group at a time in "Add new item" user interface.
- Improved assembly scanning during startup.
- Dynamic source code plugin method signature validation.
- User interface and general options refactorings.


### Release 1.2.33
-----------------
<p class="text-muted">2017-06-07</p>

Features

- Added an option to specify build parameters for Jenkins builds.
- Added an icon to AnyStatus tool window to support Visual Studio Iconizer.


### Release 1.2
--------------
<p class="text-muted">2017-05-28</p>

Features

- New Metrics and Monitors
  - Custom monitor using C#/VB.NET file.
  - SQL Server connection monitor.
  - IIS application pool monitor.
  - Network Upload/Download speed metric.
- Added a new toolbar button called "Activity Log" that opens AnyStatus pane in the Visual Studio output window.
- Custom actions like "Open in browser" and "Trigger a new build" are now disabled when the status is Error.
- AnyStatus Desktop (standalone version).
- Bold folder names.

Bug Fixes

- VS crash when opening options page after first installation.
- Help button now links to AnyStatus documentation.

[Read More](/2017/05/28/anystatus-release-1.2.html)


### Release 1.1
---------------
<p class="text-muted">2017-03-19</p>

Features

- Desktop notifications.
- Encrypted configuration file.
- Folder status summary.
- Sort statuses by priority in Color Theme options page.
- NuGet packages upgrade (scheduler, wpf toolkit, vs sdk build tools).
- Added "Queued" status to indicate a build has been queued but not started (currently used only in AppVeyor build monitor).

Bug Fixes

- Fixed folder width issue when disabled.
- Fixed TeamCity authentication bug.
- Fixed "Move Down" context menu command.
- Fixed "Remove" context menu command confirmation text.
- Changed restore default settings confirmation text.

Known Issues

- Notifications may be published more than once when using multiple Visual Studio instances.


### Release 1.0
---------------
<p class="text-muted">2017-01-31</p>

Features

- Visual Studio 2017 RC support.
- Pingdom integration.

Bug Fixes

- "Delete" changed to "Remove".


### Release 0.12
---------------
<p class="text-muted">2017-01-12</p>

Features

- Configuration change notification.
- Uptime Robot integration.
- Show "Please wait..." while Visual Studio is loading.
- Right-to-Left layout.

Bug Fixes

- Improved startup experience.
- Fixed AppVeyor build canceled status.


### Release 0.11
---------------
<p class="text-muted">2016-12-22</p>

Features

- Trigger Jenkins, TFS, AppVeyor and TeamCity builds.
- Start, stop and restart windows services.
- Collapse folders when starting.
- Update build status after triggering a build.
- Custom commands (for example, queue new build, open in browser, etc.).

Bug Fixes

- Fixed bug when duplicating TFS builds.
- Fixed keyboard navigation and context menu issues.


### Release 0.10
---------------
<p class="text-muted">2016-11-20</p>

Features

- New item/folder toolbar buttons.
- Duplicate folders.
- Added "Open in browser" option to context menu.
- Replaced status icon with vector graphics.
- Status icon indicators.
- User settings refactoring.
- UX/UI improvements.

Bug Fixes

- Set treeview inactive selection color as active.
- Changed toolbar name to AnyStatus instead of Test Toolbar.


### Release 0.9
---------------
<p class="text-muted">2016-11-03</p>

Features

- Status icon indicators.
- Added aggregated status indicators to Folders.
- Added tooltips that describes the status and type of the monitors.
- Duplicate items.
- Added Refresh button to folders.
- Enable or disable items within a group.


### Release 0.8
---------------
<p class="text-muted">2016-09-17</p>

Features

- Import and Export settings.
- Toolbar commands refactoring.
- Added a Test button to new item dialog.
- Press Delete to delete selected item.
- Detailed exception log messages.

Bug Fixes

- Fixed a critical bug in settings initialization.
- HTTP Status: treat HttpRequestException as error.
- Improved startup experience.


### Release 0.7
---------------
<p class="text-muted">2016-09-10</p>

Features

- GitHub Issue monitor.
- PowerShell Script monitor.
- Batch File monitor.
- Press F2 to rename selected item.
- Expand/Collapse toolbar buttons.
- Enable or disable Report Anonymous Usage in Options dialog.
- Enable or disable debug mode in Options dialog.
- Simplified Add New Item and Properties windows.

Bug Fixes

- Fixed TFS queued & canceled builds status color.
- Improved user settings management.


### Release 0.6
---------------
<p class="text-muted">2016-09-04</p>

Features

- TFS 2015 & Team Foundation Services build status.
- Drag-and-drop to move items between folders or to reorder items within a folder.
- Move item up/down context menu buttons.
- Pluggable health checks infrastructure.
- Basic input validation.
- Hide password characters.
- Write debug information to output window.
- Added categories to item properties.


### Release 0.5
---------------
<p class="text-muted">2016-08-26</p>

Features

- Windows Service status monitor.
- Added optional credentials to Jenkins build.
- AppVoyer build status.
- Edit health check properties.
- Enable/Disable health check.
- Refresh all health checks toolbar button.

Bug Fixes

- UX/UI improvements.


### Release 0.4
---------------
<p class="text-muted">2016-08-23</p>

Features

- TeamCity build status.
- Visual Studio 2013 Support.

Bug Fixes

- Fixed a critical bug in New Item Wizard.


### Release 0.3
---------------
<p class="text-muted">2016-08-21</p>

- Refresh monitor status.
- TCP port monitor.


### Release 0.2
---------------
<p class="text-muted">2016-08-20</p>

Features

- Ping health check.


### Release 0.1
---------------
<p class="text-muted">2016-08-19</p>

Features

- Initial release.
- Folder structure.
- Jenkins build status.
- HTTP health check.
