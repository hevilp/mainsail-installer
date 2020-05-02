# mainsail-installer
This is an install script to setup [Klipper](https://github.com/KevinOConnor/klipper), the [Klipper API](https://github.com/Arksine/klipper/tree/work-web_server-20200131), and the [Web Interface](https://github.com/meteyou/mainsail) on a clean SD card image with Raspbian

# How to Install
Copy the contents of this repository to your home directory on the pi.  
Run `chmod +x ~/mainsail-installer/mainsail-installer.sh` to make executable.  
Run `~/mainsail-installer/mainsail-installer.sh` to start the install.  

# Known Issues
Copy a working `printer.cfg` with the edits from [here](https://github.com/meteyou/mainsail#configure-klipper-api) to your home directory. The script will copy a sample `printer.cfg` currently but it may cause issues in its current form.  
The install process for Klipper will only compile the MCU firmware. You may get connection errors if the firmware on the board is not already flashed for Klipper.  
Installer will only report a wireless IP address at the end. If you have a wired connection, it won't display an address.
Error detection isn't terribly robust.
