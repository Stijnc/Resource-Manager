# Create a VM and select the storage account type 
<a href="https://portal.azure.com/#create/Microsoft.Template/uri/" target="_blank"> 
    <img src="http://azuredeploy.net/deploybutton.png"/> 
</a> 
Using this template you can deploy 1 VM, but specify the storage account type. The VM is a fixed size DS1 
 
## Additional characteristics
 - Location is fixed to West Europe
 - Choose the storage account type
	- standard LRS (Default)
	- Standard-ZRS
    - Standard-GRS
    - Standard-RAGRS
    - Premium-LRS
 - one virtual network predefined 
 - Only Windows Servers, limited to: 
	- 2012 R2 Datacenter 
	- 2008-R2-SP1 
	- 2012-Datacenter 
	- 2012-R2-Datacenter (Default) 
	- Windows-Server-Technical-Preview 
	- Subnet Range: 10.0.0.0/16 - 1 Subnet 
		- Subnet-1 (10.0.0.0/24)
