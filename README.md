stealth scan detection daemon
=====================

this stealth scan detection daemon sniffs packets in the background using the packet
capture library (pcap), filtering out packets with certain flags on, pointed
at the host computer and logs information to files in ```/var/logs/```.

***dependancies***: neato (part of the graphviz pkg.)

compile pdefdev.c and scan_detector.c, then use the bash wrapper program scandd.

usage: ./scandd [start | stop | status | clear | png]

start - run the scan_detector

stop - kill the scan_detector process

status - print the scan detector's logs

clear - erase the scan detector's logs

png - draw a graph of captured scans
