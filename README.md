# Firewall Iptables
Simple iptables script to small office, company or home network
This script have simple rules, but they are also very important!

## Installation
Download with git.
```bash
#I like to put my scripts on /etc/.
#If you want to put the scripts in another directory, change the directory in the firewall-restart file
cd /etc/
git clone https://github.com/devve2kkcc/firewalliptables.git
```
## Usage
```bash
 cd /etc/firewalliptables
# Change ports you want open in firewall file with any editor! (nano, vi, vim)
 chmod +x *
 ./firewall
```

## Save rules Permenant
### Debian-based distro
```bash
sudo apt install iptables-persistent
sudo /etc/init.d/netfilter-persistent save
```
### RHEL / CentOS distros
```bash
sudo chkconfig iptables on
sudo service iptables save
```
