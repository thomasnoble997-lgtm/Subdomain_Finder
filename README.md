# Subdomain_Finder
A lightweight, interactive Bash script for fast passive subdomain enumeration using Certificate Transparency logs. No API keys required!
🔍 Interactive Subdomain Finder (sub-finder)

An interactive, lightweight, and fast Bash tool designed for passive subdomain enumeration using Certificate Transparency (CT) logs. It requires no API keys and allows you to quickly discover subdomains directly through an easy-to-use terminal interface.

✨ Features

⚡ Passive Enumeration: Gathers subdomains rapidly without sending direct traffic to the target infrastructure via crt.sh.

💬 Interactive Terminal UI: Prompts for the domain name upon execution—no complex CLI arguments needed.

🧹 Automatic Deduplication & Cleaning: Cleans up output by stripping wildcard records (*.domain.com), sorting results, and filtering out duplicates.

🛠️ Zero Configuration: Works out-of-the-box using standard Unix tools (curl, python3, and bash).

📋 Requirements

Ensure you have the following installed on your system:

bash

curl

python3

🚀 Installation

Clone the repository:

git clone https://github.com/YOUR_USERNAME/sub-finder.git
cd sub-finder


Make the script executable:

chmod +x sub-finder


(Optional) Install system-wide as a command:

sudo mv sub-finder /usr/local/bin/sub-finder


💻 Usage

Simply run the tool and type your target domain when prompted:

./sub-finder


Example Session:

========================================
          INTERACTIVE SUB-FINDER        
========================================
Enter target domain (e.g., example.com): target.com

[*] Querying Certificate Transparency logs for: target.com...
--------------------------------------------------
admin.target.com
api.target.com
blog.target.com
dev.target.com
mail.target.com
staging.target.com
--------------------------------------------------
[*] Subdomain scan complete.


📂 Project Structure

.
├── sub-finder      # Main interactive Bash script
└── README.md       # Project documentation


⚠️ Disclaimer

This tool is created strictly for educational purposes, security research, and authorized bug bounty hunting. Ensure you have explicit authorization before scanning target organizations or networks.
