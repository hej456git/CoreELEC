## Full3D frame-packing support

This fork contains an experimental implementation for converting **Full-SBS (3840×1080)** and **Full-TAB/OU (1920×2160)** 3D video into genuine **1080p HDMI frame-packed 3D**, preserving full 1920×1080 resolution per eye.

The implementation uses Kodi to detect the Full3D layout and the Amlogic video pipeline to feed the two eye regions through VD1/VD2 into the existing HDMI frame-packing path. Normal MVC frame-packed 3D playback is retained.

Current testing has been performed on a **Nokia Streaming Box 8010 (Amlogic S905X4)** with CoreELEC 22 and an active-shutter 3D projector. Full-SBS, Full-TAB and MVC playback have all been tested successfully.

The Full3D work is currently maintained in the `full3d` branch and uses corresponding `full3d` branches of the [xbmc](https://github.com/hej456git/xbmc/tree/full3d) and [common_drivers](https://github.com/hej456git/common_drivers/tree/full3d) forks.

For project notes, releases and test material, see:
[coreelec-full3d-framepacking](https://github.com/hej456git/coreelec-full3d-framepacking)


# CoreELEC

CoreELEC is a 'Just enough OS' Linux distribution for running the award-winning [Kodi](https://kodi.tv) software on popular low-cost hardware. CoreELEC is a minor fork of [LibreELEC](https://libreelec.tv), it's built by the community for the community. [CoreELEC website](http://coreelec.org).

**Documentation**

- [CONTRIBUTING.md](CONTRIBUTING.md) — how to report issues and submit pull requests
- [STANDARDS.md](STANDARDS.md) — coding standards for build scripts and package files
- [packages/README.md](packages/README.md) — detailed guide to `package.mk` structure and variables

**Issues & Support**

Please report issues via the CoreELEC [Forum](https://discourse.coreelec.org).

**Donations**

At this moment we do not accept Donations. We are doing this for fun not for profit.

**License**

CoreELEC original code is released under [GPLv2](https://www.gnu.org/licenses/gpl-2.0.html).

**Copyright**

As CoreELEC includes code from many upstream projects it includes many copyright owners. CoreELEC makes NO claim of copyright on any upstream code. Patches to upstream code have the same license as the upstream project, unless specified otherwise. For a complete copyright list please checkout the source code to examine license headers. Unless expressly stated otherwise all code submitted to the CoreELEC project (in any form) is licensed under [GPLv2](https://www.gnu.org/licenses/gpl-2.0.html). You are absolutely free to retain copyright. To retain copyright simply add a copyright header to each submitted code page. If you submit code that is not your own work it is your responsibility to place a header stating the copyright.
