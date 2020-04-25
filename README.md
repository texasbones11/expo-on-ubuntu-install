# expo-on-ubuntu-install
How to install npm, nodejs and Expo on Ubuntu 20.04


## Ubuntu 20.04
### VirtualBox Configuration
Install ubuntu desktop 20.04 ISO on a new VM
Configure the VM for 4GB RAM, 2 CPU Threads.
Configure networking for the VM to `Bridged Adapter`
### Ubuntu configuration
Install the following packages:
```bash
sudo apt-get install virtualbox-guest-dkms virtualbox-guest-utils virtualbox-guest-x11 vim git curl htop npm
```
This will have installed an older version of nodejs. We need nodejs > v12
### Nodejs and Expo install
```bash
curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
sudo apt-get install -y nodejs
```
```bash
sudo npm install -g expo-cli
```

## Create an Expo project
```bash
expo init <project-name>
cd <Project-name>
npm start
```
## Expo Phone App
Download the expo app from the phone app store. Scan the QR code using your phone and the running expo browser window on your computer.
