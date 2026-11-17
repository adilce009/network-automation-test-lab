# network-automation-test-lab
Containerized network lab for automating and verifying routers with gNMI, NETCONF, iPerf and tcpdump.
**Status: In progress (started November 2026).** This README outlines the project plan; code and results will be added as each stage is completed.

## Overview
A lightweight, containerized lab for practicing network automation and system-level testing. It emulates a small routed network and automates device configuration, telemetry collection and verification using modern model-driven interfaces.

## Planned topology
```
[host1] ── [FRR router 1] ── [SR Linux] ── [FRR router 2] ── [host2]
```
- **Nokia SR Linux:** the device under automation (gNMI, YANG)
- **FRR routers:** OSPF routing
- **Linux hosts:** traffic generation and packet capture

## Tools
Docker · containerlab · Nokia SR Linux · FRR · gNMI/gRPC (gnmic) · NETCONF (Python, ncclient) · YANG · JSON/XML/YAML · iPerf · tcpdump · Wireshark · Python

## Roadmap
- [ ] Deploy topology with containerlab and verify OSPF adjacency
- [ ] Read and push configuration over gNMI (gnmic and Python)
- [ ] Stream interface telemetry with gNMI Subscribe
- [ ] Automate configuration over NETCONF (ncclient)
- [ ] Measure throughput with iPerf and capture traffic with tcpdump
- [ ] Build a requirements-based verification matrix with pass/fail results

## Author
Adil Mahmud
