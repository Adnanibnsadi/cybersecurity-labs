# Cybersecurity Labs

A documentation-first portfolio of authorized security labs completed in isolated
virtual machines and Cisco Packet Tracer. The collection focuses on network
behavior, endpoint risk, observable evidence, and defensive interpretation.

> [!IMPORTANT]
> Every exercise in this repository was performed in an isolated, controlled
> environment using systems owned by the author or purpose-built simulations.
> Use security tools only on systems you own or have explicit permission to test.

## Lab Index

| Lab | Focus | Environment | Evidence |
| --- | --- | --- | --- |
| [Threat Landscape in Packet Tracer](Cisco-Packet-Tracer-Threat-Landscape/README.md) | Weak router configuration, phishing and ransomware scenarios, rogue wireless access, and DNS manipulation | Cisco Packet Tracer | Completed activity file and 19 screenshots |
| [Controlled ICMP Traffic](icmp-scapy-lab/README.md) | ICMP Echo traffic generation and packet observation | Kali Linux, Ubuntu Linux, Scapy, and `tcpdump` | 21-second 1080p recording |
| [Keylogging Risk Demonstration](keylogger-lab/README.md) | Keystroke-capture risk and endpoint defenses | Kali Linux and Windows 10 VMs | Two screenshots |
| [Windows Persistence and Detection](persistence-lab/README.md) | Registry-based autostart behavior and monitoring opportunities | Kali Linux, Windows 7, and VMware Workstation | Two screenshots with lab addresses redacted |
| [Reverse TCP Communication](reverse-tcp-lab-report/README.md) | Outbound connection behavior and network-monitoring concepts | Kali Linux, Ubuntu Linux, and VMware Workstation | Topology diagram and endpoint screenshots |

## What This Repository Demonstrates

- Safe lab scoping and virtual-machine isolation
- Packet-level reasoning with ICMP traffic
- Network and wireless configuration review
- Analysis of phishing, ransomware, rogue access point, and DNS risks
- Recognition of keylogging and persistence artifacts
- Defensive controls such as segmentation, least privilege, endpoint monitoring,
  egress filtering, and security awareness
- Evidence-based technical documentation

## Evidence Standard

Each lab write-up separates four things that are easy to blur together:

1. **Scope** — where the activity was performed and what was authorized.
2. **Method** — a high-level description of the exercise without deployable
   payloads or copy-and-paste attack instructions.
3. **Evidence** — the screenshots, recording, or simulation file that support the
   observations.
4. **Limitations** — what the available evidence does not establish.

The artifacts are learning records, not a penetration-test report or a claim of
production security validation. No live targets, credentials, source payloads, or
malware binaries are included.

## Repository Structure

```text
.
├── Cisco-Packet-Tracer-Threat-Landscape/
│   ├── README.md
│   ├── Investigate a Threat Landscape.pka
│   └── Screenshots/
├── icmp-scapy-lab/
│   ├── README.md
│   └── ICMP Attack.mp4
├── keylogger-lab/
│   ├── README.md
│   └── evidence images
├── persistence-lab/
│   ├── README.md
│   └── evidence images
└── reverse-tcp-lab-report/
    ├── README.md
    └── topology and endpoint images
```

## Current Limitations

- Most labs are supported by screenshots rather than packet captures, event logs,
  or exported alerts.
- Tool versions and exact VM network settings were not recorded for every lab.
- The repository does not yet include repeatable detection queries or measurable
  pass/fail criteria.
- The reverse TCP lab currently documents its topology and learning goals but does
  not include evidence of a completed connection.

## Planned Improvements

- Add sanitized packet captures and event-log excerpts where appropriate.
- Record tool versions, timestamps, and explicit success criteria.
- Add defensive detection hypotheses and validation results.
- Map findings to authoritative security-framework references.
- Use the same documentation structure for future labs.

## Authorship and Attribution

The notes and personal lab captures document work completed by **Adnan Sadi**.
Course platforms, product names, trademarks, and provider-supplied activity assets
remain the property of their respective owners.
