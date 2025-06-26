# 🧠 Bug Bounty Automation Toolkit

![GitHub release](https://img.shields.io/github/v/release/yourusername/bugbounty-automation-toolkit?style=flat-square)
![GitHub issues](https://img.shields.io/github/issues/yourusername/bugbounty-automation-toolkit?style=flat-square)
![GitHub license](https://img.shields.io/github/license/yourusername/bugbounty-automation-toolkit?style=flat-square)

## Overview
Complete Recon → Enumeration → Exploitation → Reporting automation script for bug bounty hunters.

## Features
- Subdomain enumeration using subfinder, assetfinder, amass
- Live host checking with httpx & naabu port scanning
- Endpoint discovery via gau, waybackurls, linkfinder
- Vulnerability scanning with nuclei, dalfox, gf patterns
- Subdomain takeover detection, WAF detection, DNS enumeration
- CORS, CRLF, Open Redirect, SSRF, and other vuln checks
- Auto generated ready-to-share report

## Requirements
Install dependencies:
```bash
sudo apt update
sudo apt install -y subfinder assetfinder amass httpx gau waybackurls ffuf nuclei dalfox gf linkfinder wafw00f naabu subzy dnsx python3-pip
pip3 install -r requirements.txt  # for python tools like linkfinder, corsy, secretfinder
```

## Installation
Clone the repo and set executable permission:
```bash
git clone https://github.com/yourusername/bugbounty-automation-toolkit.git
cd bugbounty-automation-toolkit
chmod +x bughunter.sh
```

## Usage
```bash
./bughunter.sh example.com
```

Output will be saved in a folder named `report_example.com` with subfolders and a summary report.

## Example Report
See the `05_report/report_example.com_YYYY-MM-DD.txt` file for a detailed bug bounty recon summary.

## License
MIT License
