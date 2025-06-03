---
aliases:
  - ip
created: 2025-03-17T14:43
updated: 2025-06-02T16:07
---

# Internet Protocol Address

## Overview

A 32-bit address that is used in all communication with a host on a [[TCP/IP Internet]].
They do not specify an individual machine, but rather a distinct connection to a network.
Thus, a single physical machine may have multiple IP addresses.

## Classes

There are five classes of IP addresses:

1. Class A, `0 <1:7, netid> <8:31, hostid>`
2. Class B, `10 <2:15, netid> <16:31, hostid>`
3. Class C, `110 <3:23, netid> <24:31, hostid>`
4. Class D, `1110 <4:31, multicast address>`
5. Class E, `11110 <5:31, reserved for future use>`

## Reserved Addresses

In addition to individual hosts on a network, an address can also be used to refer to the _network itself_.
Conventionally, the `hostid` with all bits 0 is used for this purpose.

Likewise, a “Directed Broadcast Address” is defined as an address with a `hostid` consisting of all bits 1.
This refers to _all_ hosts on a network.

A third “reserved” address is the “Limited” or “Local Network Broadcast Address”, consisting of all bits 1. This refers to all hosts on the _local_ network, independent of any assigned IP addresses.

A final “reserved” address is the “loopback” address, often called “localhost.”
It is the Class A address `127.0.0.0`, and is specifically for testing and communication between processes on the _local_ machine. According to the literature, the network address 127 should **never** appear on any network; it is essentially **not** a network address.

## Multicast Addressing
