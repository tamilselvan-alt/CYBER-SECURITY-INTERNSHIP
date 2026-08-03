# Task 1 – Basic Network Scanning with Nmap

## Objective

The objective of this task is to perform a basic network scan using Nmap to identify open ports, running services, and the operating system of a local machine or virtual machine. The findings are documented along with a basic security analysis.

## What is Nmap?

Nmap (Network Mapper) is a free and open-source network scanning tool used by network administrators and cybersecurity professionals. It helps discover devices on a network, identify open ports, detect running services, and determine the operating system of target machines.

## Why Network Scanning Matters

Network scanning is an essential part of cybersecurity because it helps:

* Discover active devices on a network.
* Identify open ports and running services.
* Detect potential security vulnerabilities.
* Verify network configurations.
* Improve overall network security.

## Tools Used

* Nmap
* Windows PowerShell (or Kali Linux Terminal)
* Local Machine / Virtual Machine
* GitHub

## Installation of Nmap

### Windows

1. Download Nmap from the official website.
2. Run the installer.
3. Complete the installation using the default settings.
4. Open Windows PowerShell or Command Prompt.
5. Verify the installation:

   ```
   nmap --version
   ```

### Kali Linux

Nmap is pre-installed. If needed, update it using:

```bash
sudo apt update
sudo apt install nmap
```

## Commands Used

### 1. Basic Scan

```bash
nmap <Target_IP>
```

### 2. Service Version Detection

```bash
nmap -sV <Target_IP>
```

### 3. Operating System Detection

```bash
sudo nmap -O <Target_IP>
```

## Scan Results

The detailed scan results are available in:

* `nmap_scan_results.txt`

## Security Analysis

For every open port discovered:

* Identify the service running.
* Explain the purpose of the service.
* Mention whether the service may introduce a security risk if left exposed.
* Recommend basic security measures such as closing unused ports, updating services, and restricting unnecessary access.

## Screenshots

The `screenshots` folder contains:

* Basic Scan Output
* Service Version Scan Output
* OS Detection Scan Output

## Repository Files

```text
Task1-Nmap/
│
├── README.md
├── nmap_scan_results.txt
└── screenshots/
    ├── basic_scan.png
    ├── service_version_scan.png
    └── os_detection_scan.png
```

## Ethical Use

This scan was performed only on a local machine or virtual machine owned by me or used with proper authorization. No external or production systems were scanned.

## Conclusion

This task demonstrates the use of Nmap for basic network reconnaissance. The scan identified active services, open ports, and operating system details, helping to understand potential security risks and the importance of regular network assessments.
