COMP3010 Set Exercise – PCAP Analysis
Author: Shane Thompson
Module: COMP3010 – Security Operations & Incident Management

Overview

This repository documents my analysis of a network intrusion incident provided as part of the COMP3010 Set Exercise. The investigation was performed using Wireshark to identify the infected system, analyse how the infection occurred, and determine the type of attack involved.

Tools & Methodology

Primary Tool: Wireshark

Supporting Tools: Linux terminal (unzip -l, packet export)

Approach:

Applied display filters to isolate HTTP, HTTPS, DNS, and SMTP traffic.

Identified malicious domains, infection timeline, and exfiltration activity.

Verified findings using packet timestamps and extracted evidence.

Key Findings

Initial infection: attirenepal.com → downloaded documents.zip

Malware file: chart-1530076591.xls

Command and Control servers: 185.106.96.158, 185.125.204.174

Post-infection beaconing: maldivehost.net

Email leakage: SMTP traffic containing credentials (base64 encoded)
