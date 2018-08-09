# Bash setup script for Ubuntu servers
[![Build Status](https://travis-ci.org/jasonheecs/ubuntu-server-setup.svg?branch=master)](https://travis-ci.org/jasonheecs/ubuntu-server-setup)

This is a setup script to automate the setup and provisioning of Ubuntu servers. It does the following:
* Adds a new user account with sudo+lxc access (+adds lxc group)
* Adds a public ssh key for the new user account NO IT DOESNT
* Disables password authentication to the server NO IT DOESNT
* Deny root login to the server
* Setup Uncomplicated Firewall
* Create Swap file based on machine's installed memory
* Setup the timezone for the server (Default to "Asia/Singapore")
* Install Network Time Protocol

# Installation
SSH into your server and install git if it is not installed:
```bash
apt-get update
apt-get install git -y
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