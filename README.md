# pfblockerNG-feeds
If you followed the instructions in [Proxmox Node Building](https://github.com/ahuacate/proxmox-node#proxmox-node-building) then you've installed pfSense and enhanced your firewall with pfBlockerNG add-on.

You've also learnt how to add feeds to block malicious and phishing websites, invasive code and more in the section shown in [Configure DNSBL feeds](https://github.com/ahuacate/proxmox-node/blob/master/README.md#84-configure-dnsbl-feeds).

But to get pfBlockerNG firewall really working you might want to consider adding the following lists.

## 1.0 My pfBlockerNG DNSBL Custom Domain Whitelist
This section is important. Sometimes a domain blocklist includes URLs that you want to access. Instead of looking for the block list culprit you can simply add the domains that should not be blocked to a whitelist. 

Simply go to pfSense WebGUI `Firewall` > `pfBlockerNG` > `DNSBL Tab`  and scroll down to `DNSBL Whitelist Section` and you should see a box to add URLs. My list is shown below and I do my best to keep it updated. Simply Cut & Paste into the `DNSBL Whitelist Section`.

```
spotify.com
device.svc.ubnt.com # UniFi Cloud
```

## 2.0 Supratim Sanyal Consolidated IP and DNSBL Blocklists
This guy has kindly made available a hourly updated consoldated list of IP addresses to the public. Simply add this [Consolidated IP address Blocklist](http://sanyalnet-cloud-vps.freeddns.org/blocklist.txt).

## 1.0 Supratim Sanyal Monster List
This guys blocklists have been developed over the years and seem to have settled down to a functional set of IP and DNSBL blocklists. 

You can get list [HERE](https://supratim-sanyal.blogspot.com/2017/04/pfsense-pfblockerng-ultimate-list-of-ip.html).

https://www.linuxincluded.com/using-pfblockerng-on-pfsense/
