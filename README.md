![](https://github.com/malsearchs/Wifi-Hacking-AircrackNG-Cheatsheet/blob/master/logo0.jpg)  excerpts from: <https://www.aircrack-ng.org/>
# WiFi-Hacking with Aircrack-NG Suite             




Aircrack-NG is a complete suite of tools to assess WiFi network security.

It focuses on different areas of WiFi security:

+ **Monitoring:** Packet capture and export of data to text files for further processing by third party tools.
+ **Attacking:** Replay attacks, deauthentication, fake access points and others via packet injection.
+ **Testing:** Checking WiFi cards and driver capabilities (capture and injection).
+ **Cracking:** WEP and WPA PSK (WPA 1 and 2).

### Tools available in Aircrack-NG Suite

AircrackNG | Usage
------------ | -------------
airbase-ng | to configure the fake access point (AP)
aircrack-ng | 802.11 WEP and WPA/WPA2-PSK key (password) cracking program
airdecap-ng	| decrypt WEP/WPA/WPA2 capture files and can also be used to strip the wireless headers from an unencrypted wireless capture
airdecloak-ng | to remove wep cloaking from a pcap file
airdrop-n | for targeted, rule-based deauthentication of users
aireplay-ng | to generate traffic for later use in aircrack-ng for cracking WEP and WPA-PSK key
airgraph-ng | to graph the txt file (the output created by airodump with -w option)
airmon-ng | to enable monitor mode on wireless interfaces, also be used to go back from monitor mode to managed mode
airodump-ng | for packet capturing of raw 802.11 frames,  also ideal for collecting WEP IVs for use with aircrack-ng
airolib-ng | to store and manage essid and password lists, compute their Pairwise Master Keys (PMKs) and use them in WPA/WPA2 cracking
airserv-ng | its a wireless card server which allows multiple wireless application programs
airtun-ng | its a virtual tunnel interface creator
besside-ng | to crack automatically all the WEP networks in range and log the WPA handshakes
dcrack | it distributes WPA/2 PSK cracking across multiple servers
easside-ng | an auto-magic tool which allows you to communicate via an WEP-encrypted access point (AP) without knowing the WEP key
packetforge-ng | to create encrypted packets that can subsequently be used for injection
tkiptun-ng | to inject a few frames into a WPA TKIP network with QoS
wesside-ng | an auto-magic tool which incorporates a number of techniques to seamlessly obtain a WEP key


## To Set Monitor Mode [mac80211] <br />
Airmon-ng creates a new monitor mode interface as mon0 <br />
`airmon-ng start <interface name>`

To start monitor mode on a specific channel <br />
`airmon-ng start <interface name> [channel number]`

To stop and remove the monitor mode interface <br />
`airmon-ng stop <interface name>`

This command will show that the monitor mode interface is listening on the desired channel frequency <br />
`iwlist mon0 channel`


