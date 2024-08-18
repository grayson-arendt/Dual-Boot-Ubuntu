<h3><strong>Required Items:</strong></h3>

- A USB flash drive with at least 4 GB of storage (Note: This drive will be erased, so back up any important data).
- A laptop or computer running Windows 11.

<h3><strong>Summary</strong></h3>

Dual booting allows you to install another operating system alongside your existing one, like adding Ubuntu to your Windows 11 machine. This gives you access to both systems without erasing your current data—provided it's done correctly.

This guide is tailored for Windows 11 and won't work on macOS due to different compatibility issues and security features on MacBooks. If you want to dual boot on a MacBook, I can help with that separately.

Although I've never experienced data loss from dual booting, it's always good practice to back up your data on an external hard drive.

[Backing up to external hard drive (optional)](https://www.microsoft.com/en-us/windows/learning-center/back-up-files)

<h3><strong>Turning off BitLocker/Device Encryption</strong></h3>

Most Windows 11 devices have BitLocker enabled, but not all. If you can't find "Device Encryption" or "Manage BitLocker" in your search, your device likely doesn't have it.

**Note: Different Windows 11 versions may list encryption settings under "Device Encryption" or "BitLocker." Try both if needed.**

<h4><strong>Turn off Device Encryption</strong></h4>

<ol>
<li>Use the Windows search bar to search "Device encryption settings" and select "Open."</li>
</ol>

<p align="center">
  <img src="images/image1.png" width="400">
</p>

<ol start="2">
<li>Turn off the "Device encryption" toggle.</li>
</ol>

<p align="center">
  <img src="images/image2.png" width="400">
</p>

<ol start="2">
<li>Confirm by pressing "Turn off."</li>
</ol>

<p align="center">
  <img src="images/image3.png" width="400">
</p>

<ol start="4">
<li>Wait for the decryption process to complete.</li>
</ol>

<p align="center">
  <img src="images/image4.png" width="400">
</p>

<h4><strong>Turn off BitLocker</strong></h4>

<ol>
<li>Search for "Manage BitLocker" in the Windows search bar and click "Open."</li>
</ol>

<p align="center">
  <img src="images/image5.png" width="400">
</p>

<ol start="2">
<li>Click "Turn off BitLocker" under the "Operating system drive" section.</li>
</ol>

<p align="center">
  <img src="images/image6.png" width="400">
</p>

<ol start="3">
<li>Wait for the drive to decrypt fully. It might take some time. You'll see this screen when it's done:</li>
</ol>

<p align="center">
  <img src="images/image7.png" width="400">
</p>

<h3><strong>Creating a Bootable USB Flash Drive</strong></h3>

Rufus is a tool that converts your USB flash drive into a bootable drive with an operating system. After installing Ubuntu from the USB, you won’t need the drive plugged in to use Ubuntu.

<ol>
<li><a href="https://releases.ubuntu.com/jammy/ubuntu-22.04.4-desktop-amd64.iso" target="_blank">Install Ubuntu 22.04 ISO here.</a></li>
<li><a href="https://github.com/pbatard/rufus/releases/download/v4.5/rufus-4.5.exe" target="_blank">Install Rufus here.</a></li>
<li>Search for "rufus-4.5.exe" using the Windows search bar and select "Run as administrator."</li>
</ol>

<p align="center">
  <img src="images/image8.png" width="400">
</p>
 
<ol start="4">
<li>Click "Yes" to allow Rufus to make changes to your device.</li>
<li>In Rufus, select your USB flash drive from the "Device" dropdown. The drive might be labeled differently than "USB DRIVE (D:)."</li>
</ol>

<p align="center">
  <img src="images/image9.png" width="400">
</p>

<ol start="6">
<li>Click the "SELECT" button under "Boot selection."</li>
</ol>

<p align="center">
  <img src="images/image10.png" width="400">
</p>

<ol start="7">
<li>Locate and select the "ubuntu-22.04.4-desktop-amd64" file in your Downloads folder, then click "Open."</li>
</ol>

<p align="center">
  <img src="images/image11.png" width="400">
</p>

<ol start="8">
<li>Ensure the correct drive and file are selected, then click "START."</li>
</ol>

<p align="center">
  <img src="images/image12.png" width="400">
</p>

<ol start="9">
<li>Confirm by pressing "OK" for ISO Image mode.</li>
</ol>

<p align="center">
  <img src="images/image13.png" width="400">
</p>

<ol start="10">
<li>Click "OK" to erase the USB flash drive. If you have important data on it, cancel and choose a different drive.</li>
</ol>

<p align="center">
  <img src="images/image14.png" width="400">
</p>

<ol start="11">
<li>If you see this pop-up, click "OK."</li>
</ol>

<p align="center">
  <img src="images/image15.png" width="400">
</p>

<ol start="12">
<li>Wait for Rufus to finish creating the bootable USB drive.</li>
</ol>

<h3><strong>Installing Ubuntu 22.04</strong></h3>

<ol>
<li>Plug in the USB drive you just created.</li>
<li>Search for "Change advanced startup options" in the Windows search bar and click "Open."</li>
</ol>

<p align="center">
  <img src="images/image16.png" width="400">
</p>
 
<ol start="3">
<li>Click "Restart now" under "Advanced startup."</li>
</ol>

<p align="center">
  <img src="images/image17.png" width="400">
</p>

<ol start="4">
<li>Once in the advanced startup menu, choose "Use a device." You can use your mouse or arrow keys + Enter.</li>
</ol>

<p align="center">
  <img src="images/image18.png" width="500">
</p>

<ol start="5">
<li>Select your USB flash drive from the list. It might be labeled differently than "Linpus lite."</li>
</ol>

<p align="center">
  <img src="images/image19.png" width="500">
</p>

<ol start="6">
<li>Press Enter with "Ubuntu" highlighted in the menu.</li>
</ol>

<p align="center">
  <img src="images/image20.png" width="500">
</p>

<ol start="7">
<li>Choose "Install Ubuntu."</li>
</ol>

<p align="center">
  <img src="images/image21.png" width="500">
</p>

<ol start="8">
<li>Continue with the default settings on the next few pages.</li>
<li>When prompted, select your Wi-Fi network and enter the password.</li>
<li>Continue until you reach this page:</li>
</ol>

<p align="center">
  <img src="images/image22.png" width="500">
</p>

<ol start="11">
<li>Ensure "Install Ubuntu alongside Windows Boot Manager" is selected, then click "Continue."</li>
</ol>

<p align="center">
  <img src="images/image23.png" width="500">
</p>


<ol start="12">
<li>Drag the divider to allocate space for Ubuntu. I recommend at least a quarter of your hard drive space. Then, click "Install Now."</li>
</ol>

<p align="center">
  <img src="images/image24.png" width="500">
</p>

<ol start="13">
<li>Press "Continue" to confirm</li>
<li>Choose your time zone (Chicago) and click "Continue."</li>
<li>Enter your desired username and password, then click "Continue."</li>
<li>Wait for Ubuntu to install, then click "Restart Now."</li>
<li>Remove the USB flash drive when prompted and press "Enter."</li>
</ol>

<p align="center">
  <img src="images/image25.png">
</p>
 
<ol start="18">
<li>After restarting, the GRUB menu will appear each time you start your device. Use the arrow keys + "Enter" to choose which operating system to boot.</li>
</ol>

<p align="center">
  <img src="images/image26.png" width="500">
</p>

<ol start="19">
<li>Congratulations! You've successfully dual-booted your device. I recommend following the <a href="https://docs.ros.org/en/humble/Installation/Ubuntu-Install-Debians.html" target="_blank">ROS 2 Humble installation guide</a>. next. This installation will be done on Ubuntu, so boot into Ubuntu first. Copy and paste the commands in the Terminal (shortcut to open is Ctrl + Alt + T) one line at a time, then press "Enter."</li>
</ol>
