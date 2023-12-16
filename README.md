airport-ssid-channel
=============

If you want to get associated to a specific BSSID with Mac OS, use this fork. As I couldn't get the BSSID work directly on Monterey and Ventura with the original airport-bssid, here you can pass a combination of SSID and Channel Number to achieve something similar.

Example of usage: ./airport-ssid-channel <interface> <SSID_name> <channel_nr>
                  ./airport-ssid-channel en0 Home_network_name 11

You can find the channel number with running: sudo airport -s
Where you should choose the channel number for the BSSID which has the strongest signal (lowest -negative- number for the RSSI).

Obviously `airport` may decide at some point that the connection you forced is not "good enough" and switch to a different one. See if you can make something good out of `/System/Library/PrivateFrameworks/Apple80211.framework/Resources/airport`.
