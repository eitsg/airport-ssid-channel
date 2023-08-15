airport-ssid-channel
=============

If you want to get associated to a specific bssid with Mac OS, use this one. As I couldn't get the BSSID work directly on Monterey, as in the original fork, here you can pass a combination of ssid and channel to achieve something similar.

Obviously `airport` may decide at some point that the connection you forced connection to is not "good enough" and switch to a different one. See if you can make something good out of `/System/Library/PrivateFrameworks/Apple80211.framework/Resources/airport`.
