# netsec-test-script
Script to test prevention and detection of network threats.

Usage:
```
pip3 install -r requirements.py
python3 main.py
```

```
#1 Test connection with known bad IPs.
#2 Test connection with known bad URLs.
#3 Test TOR Exits Nodes.
#0 Exit.
Choice:
```

The script will dowload samples from OpenDBL ([EmergingThearts](http://opendbl.net/lists/etknown.list) and [Cisco Talos](http://opendbl.net/lists/talos.list)), Security.gives ([Mirai](https://mirai.security.gives/data/ip_list.txt)), [OpenPhish](https://openphish.com/feed.txt) and [SecOps-Institue Github (TOR Exit Nodes)](https://raw.githubusercontent.com/SecOps-Institute/Tor-IP-Addresses/master/tor-exit-nodes.lst) and test connection to random samples.

Results are saved to different text files on the running folder with a timestamp so you can validate detection at your FW, Proxy, SIEM, etc.

This script is Work-In-Progress, bugs and exceptions may appear, and new features may be added on the future.
