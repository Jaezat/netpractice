# NetPractice

This project was created as part of the 42 curriculum by mariacos.

## Description

NetPractice is a hands-on introduction to computer networking basics. Through a set of 10 progressive exercises, the goal is to fix a broken network setup by correctly assigning IP addresses, subnet masks, and routing table entries so that all hosts can communicate as intended.

The project builds intuition around IP addressing, subnetting, and how routers and switches move traffic across a network.

## Instructions

### Accessing the training tool

1. Download the exercise archive from the project page on the 42 intranet.
2. Extract it and open `index.html` in your browser.

### Working through the exercises

The tool offers two modes:

- **Training**, made up of 10 levels to go through in order.
- **Evaluation**, made up of 3 levels drawn at random from levels 6 through 10.

For each level:

1. Fill in the editable fields until the network setup satisfies the level's requirements.
2. Press **Check** to validate.
3. Check the log panel at the bottom if something is off, it usually points to the mistake.
4. Use **Get my config** to export your solution as a JSON file.
5. Move on to the next level once it's validated.

## Key Concepts

**Network**: a set of interconnected hosts that exchange data. Networks can be split into smaller subnetworks or joined together into larger ones.

**LAN (Local Area Network)**: devices connected within a small physical area (an office, a building), usually through a switch.

**WAN (Wide Area Network)**: a network spanning large distances, linking multiple LANs through routers. The internet is the largest example of a WAN.

**Internet**: the worldwide network of networks, all speaking the same TCP/IP protocol suite.

**TCP/IP**: the protocol suite that governs how data is packaged, addressed, and routed between hosts.

**IP address**: a unique identifier for a host on a network. In IPv4 it's a 32 bit number written as four decimal octets (e.g. `192.168.1.10`), split into a network part and a host part.

A few things worth remembering:

- The `127.x.x.x` range is reserved for loopback traffic.
- The `10.x.x.x`, `172.16.x.x` to `172.31.x.x`, and `192.168.x.x` ranges are private and not routed on the public internet.
- The lowest address in a subnet identifies the network itself.
- The highest address in a subnet is the broadcast address.

**Subnet mask**: paired with an IP address to define where the network part ends and the host part begins. It's written like an IP address, but as a run of 1 bits followed by 0 bits (e.g. `255.255.255.0`).

**Router / Gateway**: a device that passes traffic between separate networks.

**Routing table**: a list, kept by a router or host, of which gateway to use to reach a given destination network. A route of `0.0.0.0/0` is the catch all, used when nothing more specific matches.

**Switch**: forwards traffic between devices on the same LAN based on MAC address.

**The OSI model**: a 7 layer reference model for how networked communication is organized:

1. Physical: raw bit transmission over the medium.
2. Data Link: device to device delivery within one network segment.
3. Network: routing between networks, based on IP addresses.
4. Transport: reliable delivery, segmentation and reassembly.
5. Session: setting up and tearing down connections.
6. Presentation: formatting, encryption, compression.
7. Application: the protocols apps actually use to talk to each other.

## References

- NetworkChuck: [Subnetting playlist on YouTube](https://www.youtube.com/watch?v=5WfiTHiU4x8&list=PLIhvC56v63IKrRHh3gvZZBAGvsvOhwrRF)
- Microsoft Learn: TCP/IP addressing and subnetting fundamentals
- GeeksforGeeks: OSI Model overview
- GeeksforGeeks: TCP/IP in networking

## AI use

AI was used to help clarify concepts related to network and subnet masks. 