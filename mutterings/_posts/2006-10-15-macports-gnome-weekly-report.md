---
title: MacPorts / GNOME Weekly Report
date: 2006-10-15 00:00
categories: Mutterings
tags:
  - GNOME
  - MacPorts
  - Weekly Report
redirect_from:
  - /post/171305225430/macports-gnome-weekly-report
---
GNOME has sound! (Actually ever since we ported gstreamer version 0.10.0+, GNOME has had working sound if the esd output was selected in the GNOME Preferences.) This weekend I ported gnome-audio. Although it has no dependencies, and nothing depends on it except the gnome-desktop-suite metaport, it does provide a default set of sounds for the GNOME desktop.

A significant portion of the GNOME desktop is now at the version 2.16.0 specifications, although there are a couple of ports, such as gnome-applets, that just refuse to upgrade from 2.12/2.14 versions. I&rsquo;m sure they can be made to at least build, but I haven&rsquo;t figured out how yet.

There a couple of [GNOME Tasks](https://trac.macports.org/query?0_port=GNOME&0_port_mode=%7E&0_status=%21closed&col=id&col=summary&col=port&col=status&col=owner&col=type&col=priority&col=time&col=changetime) that when completed, or possibly just partially completed, will improve the quality and maintainability of the GNOME ports. I am still adding tasks as I think of them and as I think of how to write them.

I have a [port status](https://trac.macports.org/wiki/GNOMEPackageStatus) table that lists all the ports in the GNOME desktop. If anyone wants to have a go at porting a package that is not ported, or at updating the outdated ports, please do so, [file a ticket](https://trac.macports.org/newticket) with the port attached and assign it to rhwood@macports.org. Please note that if a port is listed as Broken and the port can not be found, it means that I have started working on the port, but have not yet gotten it to build or run well enough to release it to the rest of the MacPorts community.

Report 4
