<h1 align="center">  Setting Up a VPN in Azure </h1>

<p align="center">
<img src="https://its.ucsc.edu/vpn/images/vpn-banner2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<h1 align="center"> This guide shows you how to set up a VPN on an Azure Virtual Machine using Proton VPN. </h1> 

## Tools You’ll Use
- Proton VPN (free version)
- Microsoft Azure (to create a Virtual Machine)
- Remote Desktop (to connect to your VM)
- Internet Information Services (IIS)

## Operating System
- Windows 10

## Steps Overview
1. Find your local IP address.
2. Set up a Virtual Machine in Azure.
3. Find the VM’s IP address.
4. Connect to the VPN on the VM.
5. Check the IP address with the VPN on.

## Step-by-Step Instructions

### Step 1: Find Your Local IP Address
- Go to `www.whatismyipaddress.com` on your computer to see your local IP address. Save it for later.  
  <img src="https://i.imgur.com/cFxtnVJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

---

### Step 2: Set Up a Virtual Machine in Azure
- Go to `www.portal.azure.com`. Sign up for a free account if needed (it gives a $200 credit).
- Find “Virtual Machines” and create a new one.
- Choose any region you prefer. Match the settings in the images below.  
  <img src="https://i.imgur.com/K9oaS2z.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
  <img src="https://imgur.com/8WdUuXQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

- Set a username and password. Save them somewhere safe.  
  <img src="https://i.imgur.com/rXIj3Zb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

- Go to the “Networking” tab and match the settings in the image below.  
  <img src="https://i.imgur.com/egDvzHq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

- Click “Review and Create,” then “Create” after validation.

---

### Step 3: Log Into the VM and Find Its IP Address
- In Azure, go to your Virtual Machine’s page. Note its public IP address (e.g., 20.109.13.170).  
  <img src="https://i.imgur.com/ioSGruE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

- Open “Remote Desktop Connection” on your computer. Enter the VM’s public IP and log in with your username and password.  
  <img src="https://i.imgur.com/66Gvk3r.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
  <img src="https://i.imgur.com/UKHc92T.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>  
  <img src="https://i.imgur.com/obSCLLq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

- On the VM, open a web browser and go to `www.whatismyipaddress.com`. The IP should match the VM’s public IP, and the location should match the region you chose.  
  <img src="https://i.imgur.com/eqZ9inU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

---

### Step 4: Connect to the VPN on the VM
- On your computer, go to `protonvpn.com` and create a free account. Save your login details.
- On the VM, open a web browser, go to `protonvpn.com`, and log in.  
  <img src="https://res.cloudinary.com/dbulfrlrz/images/w_1200,h_605,c_scale/f_auto,q_auto/v1721663947/wp-vpn/sign-in-2/sign-in-2.png?_i=AA" height="80%" width="80%" alt="Disk Sanitization Steps"/>

- Click “Downloads” and download the Windows version of Proton VPN. Install it on the VM.  
  <img src="https://i.imgur.com/0V5GMWX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

- Open Proton VPN on the VM, log in with your account, and connect to a VPN server (e.g., in the USA).  
  <img src="https://i.imgur.com/CcSTBkW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

---

### Step 5: Check the IP Address with the VPN On
- On the VM, go to `www.whatismyipaddress.com` again. The IP and location should now match the VPN server (e.g., a USA IP).  
  <img src="https://i.imgur.com/L7CG91R.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

---

🎉 Congrats! You’ve set up a VPN on a Windows Virtual Machine. If you don’t need the VM anymore, delete it in Azure to avoid charges.
