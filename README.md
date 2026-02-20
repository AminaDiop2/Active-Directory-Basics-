# Active-Directory-Basics
This lab walks you through building Active Directory from scratch using real infrastructure  
What we will do:
#### Step1: Deploy a Windows Server VM in Azure with minimal cost  
#### Step2: Install Active Directory Domain Services (AD DS)  
#### Step3: Promote a server to a domain controller  
#### Step4: Design a simple, logical OU structure  
#### Step5: Create and manage users and security groups  
#### Step6: Understand how group membership controls access  

---

### Step1: Deploy a Windows Server VM in Azure with minimal cost    
All the steps for the deployment can be found [here](/deployment)

---

### Step2: Install Active Directory Domain Services (AD DS)  
1. Connect to the Server
  Use Remote Desktop (RDP) to connect to the server  
   - Access the Azure Portal: Go to the Azure portal and search for "Virtual machines" to find your VM.  
   - Verify Status & IP: Ensure the VM is running and note its Public IP address.  
   - Connect: Click the Connect button at the top of the virtual machine page, then select Connect > Native RDP.  
   - Download RDP File: Click Download RDP File.  
   - Run RDP File: Open the downloaded .rdp file. Click "Connect" if prompted by a security warning.  
   - Enter Credentials: When prompted, enter the username and password created when setting up the VM.  
   - Log in with the local administrator account you created earlier  

2. Open Server Manager
Server Manager should open automatically after login
If not, open it from the Start Menu

3. Add Roles and Features
Select Add Roles and Features
On the Before you begin screen, select Next
Select Role-based or feature-based installation
Select the local server (default)
4. Server Roles
Check Active Directory Domain Services
When prompted, select Add Features
No additional roles are required at this stage.

5. Features
Leave all features at their default selections
6. AD DS Information
Review the information page
Select Next
7. Confirmation
Confirm the role selection
Select Install
Wait for the installation to complete. The server does not need to reboot yet
