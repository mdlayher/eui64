eui64
=====

Command `eui64` provides a simple utility to convert an IPv6 address to an
IPv6 prefix and MAC address, or to convert an IPv6 prefix and MAC address
to an IPv6 address.

Usage
-----

```
$ ./eui64 -h
Usage of ./eui64:
  -ip="fe80::": IPv6 address or IPv6 prefix to parse
  -mac="": EUI-48 or EUI-64 MAC address to parse
```

Convert IPv6 prefix and MAC address to IPv6 address:

```
$ ./eui64 -ip fe80:: -mac 00:12:7f:eb:6b:40
IP: fe80::212:7fff:feeb:6b40
```

Convert IPv6 address to IPv6 prefix and MAC address:

```
$ ./eui64 -ip fe80::212:7fff:feeb:6b40
Prefix: fe80::
   MAC: 00:12:7f:eb:6b:40
```
