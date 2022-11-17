# Nintendo DWC Installer Script
Bash script which installs a Nintendo DWC server on your PC

## Requirements
- Linux Ubuntu 14 or upper or Linux Debian 9 or upper. Can be installed in a VPS or in a virtual machine with bridged network
- File `00000011.app`, which can be extracted from a Nintendo Wii NAND dump
- WiFi with WEP/no protection, wireless type 802.11b and frequency 2.4GHz

## Fix error "User is not in sudoers file" in Debian
- `su -`
- `apt-get install sudo`
- `usermod -aG sudo USER_NAME`
- `reboot`

## Usage
- `sudo apt-get update && sudo apt-get upgrade && sudo apt-get dist-upgrade && sudo apt-get autoremove && sudo apt-get autoclean`
- Put the script and the file `00000011.app` in the same folder
- `cd /path/to/nintendo_dwc_installer.sh`
- `./nintendo_dwc_installer.sh`

## Credits
- [shutterbug2000](https://github.com/shutterbug2000) who discovered [the flaw](https://github.com/KaeruTeam/nds-constraint)
