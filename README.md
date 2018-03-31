Netgear theme for LuCI (LEDE/OpenWRT)
========================================

Netgear is an alternative HTML5 theme for LuCI that has evolved from
luci-theme-bootstrap & luci-theme-material, in an attempt to bring a more
concise, clean and visually pleasing UX to LEDE/OpenWRT.

Issues & Updates
----------------

Found a bug? Please create an issue on GitHub:
    https://github.com/ysoyipek/luci-theme-netgear/issues

Further tests and PR's are welcome and appreciated.

Installation
------------

In time, Netgear may be included upstream by the LEDE/OpenWRT crowd,
to have it always available, for now, please select an installation method
most suited for your case to get it:

### Adding Netgear to your running LEDE/OpenWRT as ipk package

#### via LuCI

  * Go to System -> Software
  * Paste the following URL into the **Download and install package** field:
    - ipk url?
  * Press Enter or click "OK"

#### via shell

    $ cd /tmp
    $ wget ipk url?
    $ opkg install ipk filename?

### Adding Netgear to your own LEDE/OpenWRT Build

Edit your feeds.conf.default and add the following to it:

    # luci-theme-netgear
    src-git netgear git://github.com/ysoyipek/luci-theme-netgear.git

Update your build environment and install the package:

    $ scripts/feeds update netgear
    $ scripts/feeds install luci-theme-netgear
    $ make menuconfig

Go to LuCI -> Themes, select luci-theme-netgear, exit, save and build as usual.

Enable the Theme
----------------

  * Go to System -> System -> Language and Style
  * Choose Netgear in the Design selectbox


License
-------

This program is free software; you can redistribute it and/or
modify it under the terms of the GNU General Public License
as published by the Free Software Foundation; either version 2
of the License, or (at your option) any later version.
