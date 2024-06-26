---
title: MacPorts / GNOME Weekly Report
date: 2006-10-01 00:00
categories: Mutterings
tags:
  - GNOME
  - MacPorts
  - Weekly Report
redirect_from:
  - /post/171305185245/macports-gnome-weekly-report
---
This week I began porting the GNOME desktop to version 2.16.0

I have been mostly porting libraries, not applications, so until I get the entire set in sync, it is possible that some applications will either fail to build or crash until the entire set is in sync.

Port [dbus](https://dbus.freedesktop.org) has been reverted back to version 0.61 from 0.92 since dbus-glib can not build until some fundamental fixes are in on the dbus 0.9x ports. I have filed bugs with the upstream maintainer against this.

I thought that maybe I would have more to report, but it seems that perhaps I should hold off until next week, by which time, I hope to be more comfortable with the [Trac](https://trac.edgewall.org/) ticket system that has replaced [Bugzilla](https://www.bugzilla.org) on the MacPorts project.

Many things aren&rsquo;t working on my system due to the ongoing recovery from upgrading the gettext port and accidentally ripping out the older versions of that library.

Report 2
