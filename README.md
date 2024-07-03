# Project RaceSim_Ethercat README

## Overview
This project outlines the steps required to set up and run a CODESYS application on a Raspberry Pi. By following these instructions, you will be able to configure and deploy a control system using CODESYS and a Beckhoff EtherCAT module.

## Requirements
- Raspberry Pi with Raspbian installed and SSH enabled
- A desktop computer on the same network as the Raspberry Pi

## Setup Instructions

### 1. Register on the CODESYS Store
1. Go to the [CODESYS Store](https://store.codesys.com/en/) and create an account.

### 2. Download and Install CODESYS Development System
1. Download the CODESYS Development System from [CODESYS Store](https://store.codesys.com/en/).
2. Install the CODESYS Development System on your desktop.

### 3. Install CODESYS Control for Raspberry Pi
1. Download CODESYS Control for Raspberry Pi from [CODESYS Store](https://store.codesys.com/en/codesys-control-for-raspberry-pi-sl.html).
2. After downloading, double-click the file to install the necessary packages.

### 4. Download Beckhoff ESI Files
1. Download the ESI files for the Beckhoff module from [Beckhoff's Website](https://www.beckhoff.com/nl-nl/products/i-o/ethercat-box/epxxxx-industrial-housing/ep6xxx-communication/ep6224-0002.html?filter=%7B%22language%22%3A%5B%22English%22%5D%2C%22fileType%22%3A%5B%5D%2C%22media%22%3A%5B%5D%2C%22variants%22%3A%5B%5D%7D).

### 5. Import EtherCAT Project
1. Import the `.xml` file to include the EtherCAT project.
2. The project tree should now be visible.

### 6. Install EtherCAT Configuration
1. Go to `Tools` > `Device Repository` and click on the `Install` button.
2. Search for `EP6XXX.xml` to install the configuration for the EtherCAT module.

### 7. Update Raspberry Pi
1. Go to `Tools` > `Update Raspberry Pi`.
2. Fill in the credentials and IP address of your Raspberry Pi and click `Install`.

### 8. Configure Device Settings
1. After installation, double-click on the device icon to access the device settings.
2. Go to the `Communication Settings` tab and click on `Scan Network`.
3. Your Raspberry Pi should appear in the list. Select the Raspberry Pi.

### 9. Start the Application
1. To start the application, go to `Online` and click on `Login`.
2. After logging in, go to `Debug` and click on `Start`.

### 10. Stop the Application and Logout
1. When done, stop the application and log out.

### 11. Create Boot Application
1. To download the project to the Raspberry Pi, go to `Online` and click on `Create Boot Application`.

## Conclusion
By following these steps, you have successfully set up and configured a CODESYS application on your Raspberry Pi. You can now start developing and deploying your control systems with ease.

For any issues or further assistance, refer to the official CODESYS and Beckhoff documentation.
