# Create multiple VMs


<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3a%2f%2fraw.githubusercontent.com%2fStijnc%2fResource-Manager%2fmaster%2fMultipleVMsWithDatadisk%2fTemplates%2fMultipleMachinesWithDataDisk.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>

Using this template you can deploy multiple VMs with the same configuration.
It uses the copyIndex() function to map the number of VMs you want to deploy to the VirtualMachine and NetworkInterfaces.

## Additional characteristics
- one storage account, standard LRS (local, no geo replication)
- one virtual network predefined
	- Only Windows Servers, limited to:
		-2012 R2 Datacenter
		-2008-R2-SP1
        -2012-Datacenter
        -2012-R2-Datacenter (Default)
        -Windows-Server-Technical-Preview
	- Range: 0.0.0.0/16
	- 2 Subnets 
		- Subnet-1 (10.0.0.0/24)
        - Subnet-2 (10.0.1.0/24)