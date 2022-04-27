<p align="center">
  <img 
    width=50%
    height=50%
    src="https://i.imgur.com/b04QAsB.png"
  >
</p>

# Raspberry Pi network-attached storage (NAS) Server—2nd  Part
### Raspberry Pi SSD BOOT  



![YouTube](https://img.shields.io/badge/YouTube-%23FF0000.svg?style=for-the-badge&logo=YouTube&logoColor=white)![Raspberry Pi](https://img.shields.io/badge/-RaspberryPi-C51A4A?style=for-the-badge&logo=Raspberry-Pi)![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)![Mac OS](https://img.shields.io/badge/mac%20os-000000?style=for-the-badge&logo=macos&logoColor=F0F0F0)![IOS](https://img.shields.io/badge/iOS-000000?style=for-the-badge&logo=ios&logoColor=white)![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)

This Tutorial is a Part of RPI NAS Server. If you do not want ssd boot and  prefer old sd boot, skip this tutorial.

### Why do we need SSD BOOT ?
 Raspberry Pi boots up and stores all of its programs on a microSD memory card by default, which has a maximum theoretical bandwidth of 50 MBps on the Raspberry Pi 4 and just 25 MBps on prior models. In real-life, even the best microSD cards for Raspberry Pi get no faster than about 38 MBps in sequential writes.  Using an external SSD as your main storage drive could speed things up significantly.
  - Faster Boot Time
  - Longevity
 
### What are the things we need for SSD boot?
  - New OS update
  - New firmware update
  - New Bootloader
  - Compatible USB Adapters 
   Contains a huge list of compatible USB Adapters for this Project by James A. Chambers
   https://jamesachambers.com/raspberry-pi-4-usb-boot-config-guide-for-ssd-flash-drives/
  
### Before starting, we need external monitor / VNC remote desktop access or SSH access to the Raspberry Pi.
Tutorail link for VNC and SSH https://github.com/smartsreenath/Raspberry-Pi-VNC-Install
 
1. Prepairing SD Card: 
   - If you have already running pi with new OS and SSh enabled, skip these. Otherwise follow steps from this tutorial.
   - https://github.com/smartsreenath/Raspberry-Pi-VNC-Install (contains sd card setup, SSh setup and VNC install)
  
2. Prepairing SSD
   - Format SSD  in PC
3.	Download Putty and Install [Putty](https://www.putty.org/) (Click for the Link)
    - Open putty, select ssh, then enter the IP address and click open
    - IF asking any permission click accept and Enter
4.	Enter username: pi
    - Password: ***** (enter the password given during flashing raspberry pi using raspberry pi imager) (default password is “ raspberry ”)

5.	First you need update the OS. Type the below commands on putty
```sh
sudo apt update
```
```sh
sudo apt full-upgrade
```
6.	Type “Y” for yes
7.	Reboot PI, Type
```sh
sudo reboot now
```


 

 



