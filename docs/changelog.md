---
id: changelog
title: Changelog
sidebar_label: Changelog
---

## June 2021 (Codename Le Plateau)

Welcome to the June 2021 release of Snowtrack.

## Version 0.8.49

* **[File handling](https://github.com/Snowtrack/SnowFS/issues/192)** - Fixed an issue where Snowtrack failed to load a directory while it is being deleted.
* **[System Requirements](https://github.com/Snowtrack/SnowFS/issues/195)** - Snowtrack failed to operate on a new Windows installation.
* **Updates** - Implemented an auto-updater which makes it easier to stay up-to-date.

![Auto Updater](/img/changelog/auto-updater.png)

## Version 0.8.29

* **Performance** - Discarding changes is up to 10x times faster.
* **[Stability](https://github.com/Snowtrack/SnowFS/issues/183)** - Prevent errors that prevent Snowtrack from operating.
* **Manage Projects** - A *globe* icon indicates if the versions of a project are stored in the [global version database](terminology.md#version-database).

![Global Version Database Icon](/img/manage-projects-1.png)

#### Demo Projects

A new Pixelmator project got added to the **Demo Project** section in the welcome screen.
The artwork was created by Chris Hall Draws.

Instagram | [instagram.com/chrishalldraws](https://instagram.com/chrishalldraws)
Website | [chrishalldraws.com](https://chrishalldraws.com)

![Project Tiger](/img/changelog/demo-project-tiger.jpg)

## May 2021 (Codename Glenmount)

Welcome to the May 2021 release of Snowtrack.

## Version 0.8.27

* **Manage Projects** - **Manage projects** now includes projects from the *Recent Projects* list
* **[Unsaved changes](https://github.com/Snowtrack/SnowFS/issues/189)** - Improved detection heuristics for text files
* **Performance** - Restoring an older item is significantly faster
* **Application Support** - Enhanced minor bugfixes for Corel Draw and Pixelmator files
* **Sidebar** - Items can now be removed from the *Recent Project* list

![Sidebar](/img/changelog/sidebar-nav.png)

## Version 0.8.26

* **Change detection** - Improved change detection in Snowtrack UI by around 15% on MacOS and Windows
* **[Unsaved Changes](https://github.com/Snowtrack/SnowFS/issues/184)** - Snowtrack displayed unsaved changes after a failed **Save**.
* **[Application Info](https://github.com/Snowtrack/SnowFS/issues/185)** - Snowtrack can now display application names that prevent a discard operation.

![Process Info](/img/changelog/process-info.png)

## Version 0.8.25

* **MacOS Thumbnails** - Thumbnails on MacOS may fail to load
* **Performance** - Improve performance on Windows

## Version 0.8.24

* **Restore Item** - Restoring an item didn't give proper feedback on failure.
* **Links** - Fix links to the documentation
* **Other** - Fix typos

## Version 0.8.23

* **[Ignore Files](https://github.com/Snowtrack/SnowFS/pull/182)** - Files beginning with `Backup_of..*` are now excluded by default

## Version 0.8.21

* **ZBrush Support** - ZBrush Thumbnails can now be loaded on Windows
* **Cinema 4D Thumbnail** - Fixed an issue with the aspect ratio of Cinema 4D files.
* **Loading projects** - Fixed an issue where a project loaded forever.
* **Show Next Version** - Fixed an issue with the *Show Next Version* button.
* **Delete versions** - Fixed an issue where versions couldn't be deleted.
* **Localization** - Fixed several typos

## Version 0.8.19

* **Breadcrumbs** - Fixed an issue with the breadcrumb bar that prevented loading projects

* **[Only moves files to trash when needed](https://github.com/Snowtrack/SnowFS/issues/178)** - Items are moved only to trash if they don't have a shadow copy in the version database, otherwise they will be deleted.
* **Navigation** - Fixed an issue with mouse button navigation

## Version 0.8.12

* **Timestamps in versions** - Better heuristic when to display "*X minutes ago*" and the full date.

## Version 0.8.10

* **Performance Saving** - Creating a new version with files >4GB is 15% faster than before.
* **Menus** - Added *Changelog* and *Discord* item to the menu

## Version 0.8.9

* **macOS 10.13 Support** - The minimum requirement for Snowtrack was lowered to macOS 10.13 High Sierra.
* **Download Progress** - Downloading demo projects continues while switchting to another page.
* **Manage Projects** - Paginator removed from the *Manage Projects* view.
* **Not all files are restored on Windows** - In some cases restoring an item didn't update the file in the working directory.
* **Notifications** - Notifications within the app are covered by the loading screen.
* **All binaries are now code-signed** - Snowtrack contains a few helper tools of which all are now code-signed on Windows and macOS.
* **[Upgraded to SnowFS v0.9.2](https://github.com/Snowtrack/SnowFS/commit/b501422037fb78817bec6fc9bf37611ae1a8385a)** - All latest changes are now merged into Snowtrack

#### Demo Projects

Snowtrack now comes with 2 new demo projects, one for Blender, and another for Affinity Photo.
They can both be downloaded through the *Welcome Screen* within Snowtrack.

![Project Donut](/img/changelog/demo-project-donut.jpg)

![Affinity Photo](/img/changelog/affinity.jpg)

## Version 0.8.7

* **Tracks** - Tracks are now visualized by a graph instead of a combo-box.
* **[Performance impact when items are ignored](https://github.com/Snowtrack/SnowFS/issues/175)** - Adding a file to the 
* **[Creating version while Windows is still copying files](https://github.com/Snowtrack/SnowFS/issues/165)** - Snowtrack didn't always detect write access by the Windows File Explorer
* **Additional mouse support buttons** - Navigation buttons on your mouse can now be used within Snowtrack.
* **Keep file suffixes in version database** - Files in the object database will now keep there suffix to raise transparency.


#### Performance

Snowtrack is heavily optimized to load projects with several thousand files. Loading or scrolling just became super smooth.

#### New Version

![New Performance](https://www.snowtrack.io/wp-content/uploads/2021/05/new-performance.gif)

#### Old Version

![Old Performance](https://www.snowtrack.io/wp-content/uploads/2021/05/old-performance.gif)

---

## April 2021 (Codename Verdun)

Welcome to the April 2021 release of Snowtrack.

## Version 0.8.4

* **[Fix file access collisions](https://github.com/Snowtrack/SnowFS/issues/148)** - Handle situation when SnowFS and an external process access the same file
* **[Errors while creating a new version](https://github.com/Snowtrack/SnowFS/issues/154)** - Undefined behaviour when a project item is deleted while a version is created
* **[High memory consumption when saving](https://github.com/Snowtrack/SnowFS/issues/145)** - Saving a lot of files causes Snowtrack to consume several hundred MB of memory
* **[Stall of creating new version](https://github.com/Snowtrack/SnowFS/issues/142)** - On some machines Snowtrack doesn't return to its UI
* **[Discarding changes doesn't clean up empty directories](https://github.com/Snowtrack/SnowFS/issues/139)** - When a change is discarded, empty directories might be left behind.
* **OS Thumbnails** - Native thumbnails from Windows and macOS are used.

#### Thumbnail Support

Added thumbnail support for **ZBrush**.


![ZBrush Thumbnails](https://www.snowtrack.io/wp-content/uploads/2021/05/Ev7xWYEWQAEEC1q-1024x732.jpg)

---

## Older Versions

This is the end of the public changelog.