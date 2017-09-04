
####################################################################
        DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
                    Version 2, December 2004
 Copyright (C) 2016 Vahid Mardani
 Everyone is permitted to copy and distribute verbatim or modified
 copies of this license document, and changing it is allowed as long
 as the name is changed.
            DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
   TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
  0. You just DO WHAT THE FUCK YOU WANT TO.
####################################################################
Fixing bluetooth stereo headphone/headset problem in ubuntu 16.04 and also debian jessie, with bluez5.
Workaround for bug: https://bugs.launchpad.net/ubuntu/+source/indicator-sound/+bug/1577197
Run it with python3.5 or higher after pairing/connecting the bluetooth stereo headphone.
Only works with bluez5.
See `python3.5 a2dp.py -h`.
Shorthands:
    $ alias speakers="a2dp.py 10:08:C1:44:AE:BC"
    $ alias headphones="a2dp.py 00:22:37:3D:DA:50"
    
    $ speakers
Check here for the latest updates: https://gist.github.com/pylover/d68be364adac5f946887b85e6ed6e7ae
Change Log
----------
- 0.2.5
  * Mentioning [mac] argument.
- 0.2.4
  * Removing duplicated devices in select device list.
- 0.2.3
  * Matching ANSI escape characters. Tested on 16.10 & 16.04
- 0.2.2
  * Some sort of code enhancements.
- 0.2.0
  * Adding `-V/--version`, `-w/--wait` and `-t/--tries` CLI arguments.
- 0.1.1
  * Supporting the `[NEW]` prefix for devices & controllers as advised by @wdullaer
  * Drying the code.
"""