The officially supported release is 16.04 at the moment.

1. Download and run installation script:
`wget https://raw.githubusercontent.com/golemfactory/golem/develop/Installer/Installer_Linux/install.sh`
2. Make sure that script can be executed
`chmod +x install.sh`
3. Launch script
`./install.sh`
4. You might be asked for root password
5. If any dependencies needs to be installed, you will be asked if you want to install them. We strongly recommend to agree.
6. When the script terminates, the program, along with dependencies, will be installed. All you need to do is to restart your PC.
6. To make sure you can run golem without `sudo` run `$ sudo usermod -aG docker $USER` Warning: The docker group grants privileges equivalent to the root user. For details on how this impacts security in your system, look up: Docker Daemon Attack Surface.