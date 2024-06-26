---
title: Gimp on Mac OS X without X11 from MacPorts
date: 2007-11-20 00:00
categories: Mutterings
tags:
  - GIMP
  - GNOME
  - macOS
  - MacPorts X11
redirect_from:
  - /post/171859583235/gimp-on-mac-os-x-without-x11-from-macports
---
[![](/assets/2007-11-20-gimp.png){:width="300px"}](/assets/2007-11-20-gimp.png)

A screenshot of [Gimp](https://www.gimp.org/) running on [Mac OS X](https://www.apple.com/macosx) (version 10.4) without [X11](https://en.wikipedia.org/wiki/X11) and installed using [MacPorts](https://www.macports.org/)

## Build It!

```
sudo port install poppler +quartz
sudo port install gimp2 +no_python
sudo port install gimp +quartz
```

If that fails, this should work:

```
sudo port clean --all all
sudo port install cairo +quartz +no_x11
sudo port install poppler +quartz
sudo port install gail +quartz
sudo port install gimp2 +no_python
sudo port install gimp +quartz
```

## Notes

* I did not have X11 installed on my computer. If X11 is installed on your computer, your milage may vary.
* The supporting application jp2 crashes when Gimp is launched. Don&rsquo;t know why.
* Python support is disabled, so no scripting or plugins are available in that language.
* Further issues with this procedure should be hashed out in the [MacPorts Users Mailing List](https://lists.macports.org/mailman/listinfo/macports-users)

__UPDATE:__ I tweaked the build instructions to resolve a problem with the Gimp application launcher.

__UPDATE:__ Added a missing build instruction.
