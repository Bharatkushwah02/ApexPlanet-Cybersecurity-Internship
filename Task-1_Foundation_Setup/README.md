# ApexPlanet Internship - Task 1: Foundation & Environment Setup

## 📌 Objective
Build strong cybersecurity fundamentals and set up a professional Kali Linux lab environment for penetration testing practice.

---

## 🔍 Overview
This guide explains how to install a Kali Linux virtual machine using VMware or VirtualBox and prepare it for lab use.

## ✅ Prerequisites
- Windows PC with virtualization support enabled
- VMware Workstation or VirtualBox installed
- At least 20 GB of free disk space for the Kali VM
- Internet access to download the Kali Linux ISO

## 🧰 Tools Used
- VMware Workstation or VirtualBox
- Kali Linux ISO from the official website

## 📝 Steps to Install Kali Linux

### 1. Install virtualization software
1. Install VMware Workstation: https://www.vmware.com/info/workstation-pro/evaluation
2. Or install VirtualBox: https://www.virtualbox.org/

### 2. Download Kali Linux ISO
1. Download the Kali Linux ISO from the official website:
   - https://www.kali.org/get-kali/#kali-platforms

### 3. Create a new virtual machine
1. Open VMware (or VirtualBox) and choose **Create a New Virtual Machine**.
2. Select **Installer disc image file (ISO)** and browse to the Kali Linux ISO.

   ![Browse ISO](images/Browse_ISO.png)

3. Choose the operating system type:
   - **Linux**
   - **Ubuntu 64-bit**

   ![Select OS](images/Select_OS.png)

4. Enter a name for the VM and choose the storage location.
   - Make sure the drive has enough free space.

   ![Name and Location](images/Name_%26_Location.png)

5. Assign disk size for the VM.
   - Minimum: **20 GB**
   - Increase if your system allows it.

   ![Enter disk size](images/Enter%20disk%20size.png)

6. Optionally customize hardware settings, or continue with defaults.

   ![Customize hardware](images/Customize.png)

7. Finish the virtual machine creation.

### 4. Start the virtual machine
1. Power on the VM.
2. Select **Graphical install** and press Enter.

   ![Graphical install](images/select1st.png)

### 5. Install Kali Linux
1. Choose your language and click **Continue**.
2. Select your location and click **Continue**.
3. Select keyboard layout and click **Continue**.
4. Enter the hostname for the VM.

   ![Hostname](images/hostname.png)

5. Enter a domain name or skip this step.
6. Create a user account and password.

   ![Username](images/username.png)
   ![Confirm username](images/username1.png)
   ![Set password](images/Set%20the%20password.png)

7. Select your time zone and click **Continue**.

### 6. Partition the disk
1. Choose **Guided - use entire disk**.
2. Continue through the partitioning steps.

   ![Partition disk](images/partition.png)

3. Confirm and write changes to disk.

   ![Confirm partition](images/partition2.png)

4. Continue with the default software selection.

   ![Software selection](images/Software_selection.png)

5. When prompted, install the GRUB boot loader.

   ![GRUB loader](images/Grub.png)

6. Select **/dev/sda** for the boot loader location and continue.

### 7. Complete installation
1. Wait for the installation to finish.
2. Reboot the VM.
3. Log in using the username and password created earlier.

   ![Kali Dashboard](images/Kali%20Dashboard.png)

## 📌 Final Notes
- Use this Kali VM for cybersecurity practice, vulnerability scanning, and penetration testing labs.
- Keep the VM tools and Kali Linux updated.
- Do not use this environment for unauthorized activities.

---

## 📂 File Structure
- `README.md` - this installation guide
- `images/` - screenshot files used in the guide

