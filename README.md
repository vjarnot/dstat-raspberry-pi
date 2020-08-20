Original README.md below. My change is simple: add some parentheses at line 12.

You don't actually need this plugin, generally speaking, as the thermal plugin that's bundled with dstat does work with the Raspberry Pi. I just happen to like this one's output format better.

My preferred alias for dstat: 

    alias ds='dstat -tlrvn --rpi-thermal 10'

dstat has been, unfortunately, abandoned by its creator; a result of RedHat creating pcp-dstat aliased to dstat. Be aware that you may unintentionally install pcp and pcp-dstat on some Linux distributions even though you're actually intending to install real dstat.

Original:

dstat-raspberry-pi
==================

dstat plugins for Raspberry Pi

Copy to one of
* ~/.dstat
* /usr/share/dstat/
* /usr/local/share/dstat/

and run something like 

    dstat --time -a --cpufreq --rpi-thermal 5

