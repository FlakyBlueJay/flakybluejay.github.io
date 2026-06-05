---
title: Fix for Arch users with broken Geoclue
date: 2026-05-31
tags:
  - Linux
  - Arch-Linux
  - CachyOS
  - KDE
  - Geoclue
description: You need to enable a URL.
---
Just a quick post for anyone who is dealing with this and ending up finding more ideology slop on the Arch forums about “muh privacy” than any actual help. One post on the Arch Forums was even basically going “I don’t know, because I don’t use it and have no use for it because muh privacy”. *Super fucking helpful.*

It goes without saying but this also applies to distros that source location service packages (specifically `geoclue`) from Arch, such as EndeavourOS and the aforementioned CachyOS.

KDE uses location services to get things like weather, or sunrise/sunset with the blue light filter (“Night Light”), using **Geoclue**. The issue here is that Arch-based distros do not use a web-based location service provider by default when using Geoclue. To make matters even worse, KDE is also bad at showing to the user that the location service is not working and [lets you attempt to use it anyway](https://bugs.kde.org/show_bug.cgi?id=515222).

The fix here is simple if you know how to edit configuration files (and I assume you do if you’re using Arch) - you just enable either BeaconDB or Positon inside the configuration file for Geoclue. Arch should have the URLs in the Geoclue config file already ( `/etc/geoclue/geoclue.conf`), just find the `#url=` configuration for either BeaconDB or Positon, and restart the Geoclue service (`systemctl restart geoclue`). KDE should have all the location dependent features working now.

If anyone is editing the Arch wiki or foss.wiki, feel free to add this because I likely won’t. I’m maining Windows now.