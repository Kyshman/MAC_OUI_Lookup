# **Offline MAC Address / Vendor Pairs' Lookup Script Using Wireshark OUI Database.**
----

A script inspired by [jpouellet/manuf.sh](https://gist.github.com/jpouellet/a4301a5a8c0094673c76ffa94b94ca75)

Data Source: [Wireshark Manufacturer Database](https://gitlab.com/wireshark/wireshark/-/raw/master/manuf)

For Online lookup see [Wireshark . OUI Lookup Tool](https://www.wireshark.org/tools/oui-lookup.html)

-----

**HOW-TO/USAGE**

On the first run, the db needs to be populated with:

```
./manuf.sh update
```

The above command can be repeated periodically to fetch the latest data. Whenever the update is run it shows what has changed between subsequent updates.

Check Mac Address OUI

```
./manuf.sh 00:24:44
```
You can use ":", or "." to separate the macaddress' octets.
