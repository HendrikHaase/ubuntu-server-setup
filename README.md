# Bash setup script for Ubuntu servers

This is a setup script to automate the setup and provisioning of Ubuntu servers. It does the following:
* Adds a new user account with sudo+lxd access (+adds lxd group)
* Deny root login to the server
* Setup Uncomplicated Firewall
* Create Swap file based on machine's installed memory
* Setup the timezone for the server (Default to "Asia/Singapore")
* Install Network Time Protocol

# Installation
SSH into your server and install git if it is not installed:
```bash
apt update
apt install git lxc -y
```

Clone this repository into your home directory:
```bash
cd ~
git clone https://github.com/HendrikHaase/ubuntu-server-setup.git
```

Run the setup script
```bash
cd ubuntu-server-setup
bash setup.sh
```

# Setup prompts
you'll see

# Supported versions
This setup script has been tested against Ubuntu 14.04, Ubuntu 16.04 and Ubuntu 18.04. (as per original author)

# Running tests
no