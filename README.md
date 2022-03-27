# **Offline MAC Address / Vendor pairs Lookup Script using Wireshark OUI database.**
----

A script inspired by [jpouellet/manuf.sh](https://gist.github.com/jpouellet/a4301a5a8c0094673c76ffa94b94ca75)

Data Source: [Wireshark Manufacturer Database](https://gitlab.com/wireshark/wireshark/-/raw/master/manuf)

For Online lookup see [Wireshark . OUI Lookup Tool](https://www.wireshark.org/tools/oui-lookup.html)

-----

**HOW-TO/USAGE**

On the first run the db needs to be populated with

```
./manuf.sh update
```

The command can be repeated periodically to fetch the latest data

Whenever update is run it shows what has changed between subsequent updates.

Check macaddress OUI

```
./manuf.sh 00:24:44
```

You can also use "-", or "." to separate the octets.
