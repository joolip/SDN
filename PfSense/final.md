# Summary for PfSense installation

Here you can find summary for installation of PfSense. For installing PfSense [here](https://doc.pfsense.org/index.php/Installing_pfSense) is simple instructions for that.

## Interface configurations

Wan-interface is for internet connection, Management-interface is for control traffic, Data-interface is for end-customer traffic.

![Interfaces](https://cybertrust.labranet.jamk.fi/cf2017/overflow/raw/master/pictures/interfaces2.png)

## DNS

DNS-addresses from your network.

![DNS](https://cybertrust.labranet.jamk.fi/cf2017/overflow/raw/master/pictures/dns.png)

## DHCP

DHCP-server address-scope is from **192.168.2.20** to **192.168.2.254**

![DHCP](https://cybertrust.labranet.jamk.fi/cf2017/overflow/raw/master/pictures/dhcp.png)

## Firewall rules

Traffic between Management and Data networks is blocked. See rule below.

![Firewall rules](https://cybertrust.labranet.jamk.fi/cf2017/overflow/raw/master/pictures/firewall_rules.png)

## MTU

After some six weeks of testing, we found out that 1478 is the right number. This is because VLAN (802.1Q) frame takes 22 extra bytes, increasing MTU size to total of 1522, which we need to substract from 1500 (1478 = 1500 - (1522 - 1500)) totaling MTU size back to 1500 if VLAN tag is added.

![MTU](https://cybertrust.labranet.jamk.fi/cf2017/overflow/raw/master/pictures/mtu.png)

## Captive Portal

Captive Portal configuration.

![Captive Portal1](https://cybertrust.labranet.jamk.fi/cf2017/overflow/raw/master/pictures/captive1.png)

After succesful connection, login page appears.

![Captive Portal2](https://cybertrust.labranet.jamk.fi/cf2017/overflow/raw/master/pictures/captive2.png)


