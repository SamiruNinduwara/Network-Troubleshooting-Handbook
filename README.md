# Network Troubleshooting Handbook

A practical, step-by-step guide to diagnosing and fixing the most common LAN, WLAN and WAN faults. Written as a quick field reference for network technicians and students.

**Author:** Samiru Ninduwara, Network Student, Sri Lanka

<p align="left">
  <a href="https://github.com/SamiruNinduwara/Network-Troubleshooting-Handbook/releases/download/network-troubleshooting/Network-Troubleshooting-Handbook.pdf">
    <img src="https://img.shields.io/badge/Download%20PDF-Network%20Troubleshooting%20Handbook-1B998B?style=for-the-badge&logo=adobeacrobatreader&logoColor=white" alt="Download the PDF" />
  </a>
</p>

---

## Why I made this

Knowing the theory is not enough. A technician must be able to find a fault quickly and calmly. I wrote this handbook to practise a repeatable method and to build a reference I can use in the lab and on the job.

## What is inside

| Section | Content |
|---|---|
| 1. Introduction | How the handbook is organised and how to use it |
| 2. Troubleshooting method | 7-step method and the OSI model as a map (bottom-up, top-down, divide and conquer) |
| 3. Technician's toolkit | Windows and Cisco IOS commands, and the "golden ping sequence" |
| 4. Troubleshooting guides | 12 common faults, each with Symptoms, Possible causes, Steps, Solution and Prevention |
| 5. Extended command reference | More Windows, Linux, Cisco IOS and MikroTik commands |
| 6. Quick reference tables | Private IP ranges, common ports, LED meanings, T568A / T568B colour order, cable types |
| 7. Fault log template | A table for documenting every fault you fix |

## Faults covered

1. No internet / limited connectivity
2. IP address conflict
3. DHCP not working (APIPA 169.254.x.x)
4. DNS issues
5. Slow network
6. WiFi connected but no internet
7. Cable and port problems
8. VLAN issues (devices cannot talk)
9. Router and switch configuration problems
10. Printer not reachable on the network
11. Intermittent disconnections
12. Cannot access a device remotely (SSH / Telnet)

## The method in short

1. Identify the problem
2. Establish what is normal
3. Make a theory
4. Test the theory (change one thing at a time)
5. Plan and fix
6. Verify
7. Document

**Golden ping sequence:** `127.0.0.1` -> own IP -> default gateway -> remote IP (`8.8.8.8`) -> a name (`google.com`). Stop at the first failure.

## Tools and commands referenced

- **Windows:** `ipconfig`, `ping`, `tracert`, `pathping`, `nslookup`, `arp`, `netstat`, `netsh`, `route print`
- **Linux:** `ip`, `ss`, `dig`, `mtr`, `tcpdump`, `ethtool`
- **Cisco IOS:** `show ip interface brief`, `show vlan brief`, `show interfaces trunk`, `show ip route`, `show spanning-tree`, `show ip ospf neighbor`
- **MikroTik:** `/ping`, `/tool traceroute`, `/ip dhcp-server lease print`
- **Software:** Wireshark, PuTTY, Cisco Packet Tracer

## Who is it for

- Network students (NVQ, CCNA and similar)
- Junior network technicians and help desk staff
- Anyone who wants a clear, structured way to troubleshoot a network

## Notes

- This is a learning resource. Always follow your organisation's change-control policy before changing a live network.
- Command syntax can differ between vendors and versions. Check the manual for your device.

## Feedback

Found a mistake or have a suggestion? Please open an **Issue** on this repository. I am still learning and I welcome corrections.

## Author

**Samiru Ninduwara**
Network Student | Sri Lanka
