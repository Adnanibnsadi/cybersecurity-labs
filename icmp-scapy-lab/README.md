# Controlled ICMP Traffic Generation with Scapy

## Overview

This lab examines ICMP Echo traffic at the packet level. Scapy generated traffic
from a Kali Linux virtual machine while an Ubuntu virtual machine captured and
displayed the corresponding requests and replies.

## Scope and Safety

| Component | Details |
| --- | --- |
| Traffic generator | Kali Linux VM |
| Observation host | Ubuntu Linux VM |
| Tools | Scapy and `tcpdump` |
| Protocol | ICMP |
| Network | Isolated private virtual network |

The activity used only lab-owned virtual machines. It was a short observation
exercise, not a denial-of-service test.

## Objectives

- Construct ICMP packets with a packet-manipulation framework.
- Observe Echo Requests and Echo Replies on a receiving host.
- Connect high-level reachability tests to packet-level behavior.
- Practice documenting network experiments with clear safety boundaries.

## Method

1. Place both virtual machines on the same isolated network.
2. Confirm basic connectivity and identify the correct lab interfaces.
3. Generate ICMP Echo traffic from the Kali VM at a controlled interval.
4. Observe the traffic on the Ubuntu VM with `tcpdump`.
5. Stop the activity and review the captured terminal output.

Exact addresses are intentionally omitted because they are incidental private lab
values rather than reproducibility requirements.

## Observations

- The receiving host displayed repeated ICMP Echo Requests and Echo Replies.
- Packet capture makes direction, source, destination, and message type visible in
  a way that an ordinary `ping` summary does not.
- ICMP supports useful diagnostics, so a blanket block is usually less informative
  than measured filtering, rate limiting, and monitoring.

## Evidence

- [Screen recording of the lab](ICMP%20Attack.mp4)
- Format: H.264 video with AAC audio
- Resolution: 1920 × 1080
- Duration: approximately 21 seconds

The recording shows Scapy on Kali Linux and packet observations on Ubuntu Linux.

## Defensive Takeaways

- Establish a baseline for normal ICMP volume and destinations.
- Alert on sustained or unusual patterns rather than treating every ICMP packet as
  malicious.
- Apply rate limits at suitable network boundaries when abuse is a concern.
- Retain packet captures or flow records when an investigation requires exact
  counts and timing.

## Limitations

- No `.pcap` file or packet-count summary is included.
- CPU, latency, and packet-loss effects were not measured.
- The recording demonstrates traffic generation and observation, not service
  disruption or the effectiveness of a detection rule.

## Skills Practiced

- Scapy
- ICMP fundamentals
- Linux networking
- Packet capture with `tcpdump`
- Virtual-machine networking
- Safe experiment scoping
