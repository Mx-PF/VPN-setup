# Vitual Private Network (VPN)
<p align="center">
<img src="https://its.ucsc.edu/vpn/images/vpn-banner2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<h1>VPN - Prerequisites & Installation</h1>
This tutorial outlines the prerequisites and installation of using a VPN.<br />

<h2>Environments and Technologies Used</h2>

- A VPN (We'll be using Proton VPN)
- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>STEPS INCLUDED</h2>

- STEP 1 - Locate Local IP
- STEP 2 - Setting Up VM Using Azure
- STEP 3 - Locating the IP Through the VM
- STEP 4 - Connecting to the VPN Through the VM
- STEP 5 - Locating IP Through the VPN

<h2>Installation Steps</h2>

STEP 1 - Locate your own personal IP by going to "www.whatismyipaddress.com" which will be able to show you your local IP address. We will use this later as well.
<p>

<p>
<img src="https://i.imgur.com/cFxtnVJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Next we will set up a VM on MS Azure. 
  
</p>
<br />

STEP 2 - Go to www.portal.azure.com and find Virtual Machines. (Create a free account with $200 if you need to). 

  *See the examples below for the Virtual Machine set up page.*
<p>
<img src="https://i.imgur.com/K9oaS2z.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Create the Virtual Machine in the example below and select whatever REGION you prefer. Ensure the other items are selected as shown in the next two pictures below.
(The region you choose will be the region shown within your VM while looking at your IP With out a VPN)

(Click to magnify)
<p>
<img src="https://imgur.com/8WdUuXQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

For the Username and Password you can create your custom credentials, *just make sure to save it somewhere you can easily remember*.
  
</p>
<br />

*EXAMPLE*
<p>
<img src="https://i.imgur.com/rXIj3Zb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Select the “Networking” tab towards the top of the Azure VM page and view the image below to match. 
  
</p>
<br />

*EXAMPLE*
<p>
<img src="https://i.imgur.com/egDvzHq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Then select “Review and Create”, once it passes validation select “Create” at the bottom. 
  
</p>
<br />

NEXT: At the Virtual Machine we find that the IP to the Virtual Machine is *“20.109.13.170”*. (See *EXAMPLE* below)
</p>
<br />
*EXAMPLE*
<p>

<img src="https://i.imgur.com/ioSGruE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>


STEP 3 – Log Into the VM and Find IP Address
<p>
Now that we have set up the Virtual Machine we will connecting to it using the application “Remote Desktop Connection” and input the IP address for the VM that we located in the EXAMPLE above. Next input the set credentials we set when creating the VM. Once logged in, we will open the web browser and again look up www.whatismyipaddress.com.

  
</p>
<br />

*EXAMPLE* - (*YOUR* IPs MUST MATCH)
<p>
<img src="https://i.imgur.com/66Gvk3r.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

  
</p>
<br />

*EXAMPLE* - MAC OS (*YOUR* IPs MUST MATCH)
<p>
<img src="https://i.imgur.com/UKHc92T.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/obSCLLq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

When we look up the IP address for this VM through www.whatismyipaddress.com we see what this VM is showing the location for.
  You should see the region you selected to house the VM.
</p>
<br />

*EXAMPLE*
<p>
<img src="https://i.imgur.com/eqZ9inU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

STEP 4 – CONNECTING TO VPN (Free Version)

Using the local computer go to protonvpn.com and create a free account. *Be sure to keep track of your credentials*. Once you are logged into your account, Proceed to the VM web browser to download & install the program. 

  
</p>
<br />

<p>
<img src="https://res.cloudinary.com/dbulfrlrz/images/w_1200,h_605,c_scale/f_auto,q_auto/v1721663947/wp-vpn/sign-in-2/sign-in-2.png?_i=AA" height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>
<p>

Once you have logged into your Proton VPN account on the VM, you will select “Downloads” and choose to download the “Windows” version. Once the application Proton VPN is installed we will log in using the credentials we used when setting up a free account on Proton VPN. Then connect to the VPN through the installed app. 
</p>
<br />
<img src="https://i.imgur.com/0V5GMWX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>

See *EXAMPLE* below when the steps are completed.  
  
<br />


<p>
<img src="https://i.imgur.com/CcSTBkW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

On the left hand side of the VPN you can see the country where your VPN is conected too. The image above shows the VPN being connected to an IP in the USA.
  
</p>
<br />

<p>

</p>
<p>

Next we will look at the IP again using the VM browser now that we have connected the VPN to America. The website www.whatismyipaddress.com should reflect that IP address we just saw in the VPN.
</p>
<br />
 
<p>
<img src="https://i.imgur.com/L7CG91R.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Looking back at this exercise we see that we have utilized 3 different IP addresses just from your local computer to connect to the internet.

  
</p>
<br />
🎉 Congratulations. 🎊
</p>
You have successfully downloaded, installed, and set up a VPN inside a Windows virtual machine.
</p>
If you no longer need the VM, ensure to remove it from the Asure account for unwanted charges.
