# 🛡️ Advanced Keylogger Detection System

A comprehensive Windows-based keylogger detection and analysis tool that uses behavioral analysis, signature matching, network monitoring, and VirusTotal integration to identify and report potential keylogger threats in real-time.

## 🎯 Overview

This Final Year Project (FYP) is an advanced security tool designed to detect keyloggers and malicious processes on Windows systems through multiple detection mechanisms including process monitoring, behavioral analysis, hash verification, and real-time network traffic analysis.

## ✨ Key Features

### Core Detection Capabilities
- **Real-time Process Monitoring**: Continuous scanning of running processes for suspicious behavior
- **Multi-layered Detection Engine**:
  - Signature-based detection (file names, process names, MD5 hashes)
  - Behavioral analysis (hook detection, DLL injection, registry persistence)
  - Network activity monitoring (data exfiltration, C&C communication)
  - VirusTotal API integration for online threat intelligence

### Advanced Analysis
- **Risk Scoring System**: Weighted risk assessment with multiple factors (DLL hooks, network activity, suspicious imports, etc.)
- **Network Traffic Analysis**: Deep packet inspection for keylogger-specific patterns
- **Known Malware Database**: Signatures for Ardamax, Agent Tesla, FormBook, Remcos RAT, and other popular keyloggers
- **File Integrity Checking**: MD5 hash verification against known malicious signatures

### Reporting & Visualization
- **Comprehensive HTML Reports**: Detailed detection reports with process information and risk analysis
- **Detection Timeline**: Visual timeline of threat detection events
- **Export Capabilities**: CSV and JSON export for further analysis
- **Historical Logging**: Persistent detection history with timestamps

### User Interface
- **Modern GUI**: Tkinter-based interface with real-time updates
- **Process Management**: View, analyze, and terminate suspicious processes
- **Whitelist Management**: Exclude trusted processes and directories
- **Alert System**: Real-time notifications for detected threats

## 🔍 Detection Methods

1. **Signature Matching**: Known keylogger file patterns and MD5 hashes
2. **Behavioral Analysis**: Hook detection, DLL injection, clipboard monitoring
3. **Network Monitoring**: Suspicious outbound connections and data patterns
4. **Registry Analysis**: Startup persistence and autorun entries
5. **VirusTotal Integration**: Cloud-based threat intelligence (cached for performance)

## 🛠️ Technologies Used

- **Language**: Python 3.x
- **GUI Framework**: Tkinter
- **Network Analysis**: Scapy, PyShark, dpkt
- **Windows APIs**: pywin32 (Win32 API integration)
- **Data Analysis**: pandas, matplotlib, seaborn
- **External APIs**: VirusTotal API v2
- **Cryptography**: OpenSSL, cryptography library
