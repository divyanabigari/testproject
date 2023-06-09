---
description: This template deploys multiple virtual machines with workable HA data management gateway
page_type: sample
products:
- azure
- azure-resource-manager
urlFragment: mutiple-vms-with-data-management-gateway
languages:
- json
---
# Create HA data management gateway and install on an Azure VMs

![Azure Public Test Date](https://azurequickstartsservice.blob.core.windows.net/badges/quickstarts/microsoft.datafactory/mutiple-vms-with-data-management-gateway/PublicLastTestDate.svg)
![Azure Public Test Result](https://azurequickstartsservice.blob.core.windows.net/badges/quickstarts/microsoft.datafactory/mutiple-vms-with-data-management-gateway/PublicDeployment.svg)

![Azure US Gov Last Test Date](https://azurequickstartsservice.blob.core.windows.net/badges/quickstarts/microsoft.datafactory/mutiple-vms-with-data-management-gateway/FairfaxLastTestDate.svg)
![Azure US Gov Last Test Result](https://azurequickstartsservice.blob.core.windows.net/badges/quickstarts/microsoft.datafactory/mutiple-vms-with-data-management-gateway/FairfaxDeployment.svg)

![Best Practice Check](https://azurequickstartsservice.blob.core.windows.net/badges/quickstarts/microsoft.datafactory/mutiple-vms-with-data-management-gateway/BestPracticeResult.svg)
![Cred Scan Check](https://azurequickstartsservice.blob.core.windows.net/badges/quickstarts/microsoft.datafactory/mutiple-vms-with-data-management-gateway/CredScanResult.svg)

Before deploying the template you must have the following

1. **Data Factory.** The gateway is created in the data factory. If you don't have a data factory,  see the [Create data factory](https://docs.microsoft.com/azure/data-factory/data-factory-move-data-between-onprem-and-cloud#create-data-factory) for steps to create one.
2. **Virtual Network.** The virtual machine will join this VNET. If you don't have one, use this tutorial, see [Create virtual network](https://docs.microsoft.com/azure/virtual-network/virtual-networks-create-vnet-arm-pportal#create-a-virtual-network) to create one.

[![Deploy To Azure](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.svg?sanitize=true)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fazure-quickstart-templates%2Fmaster%2Fquickstarts%2Fmicrosoft.datafactory%2Fmutiple-vms-with-data-management-gateway%2Fazuredeploy.json)
[![Deploy To Azure US Gov](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazuregov.svg?sanitize=true)](https://portal.azure.us/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fazure-quickstart-templates%2Fmaster%2Fquickstarts%2Fmicrosoft.datafactory%2Fmutiple-vms-with-data-management-gateway%2Fazuredeploy.json)
[![Visualize](https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/visualizebutton.svg?sanitize=true)](http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fazure-quickstart-templates%2Fmaster%2Fquickstarts%2Fmicrosoft.datafactory%2Fmutiple-vms-with-data-management-gateway%2Fazuredeploy.json)
    

    

When you deploy this Azure Resource Template, you will create a logical gateway in your data factory and the following resources
- Azure Virtual Machine
- Azure Storage (for VM system image and boot diagnostic)
- Public IP Address
- Network Interface
- Network Sercurity Group

This template can help you create a gateway and make it workable in azure VM. The VM must join in an exsiting VNET. You will see the new gateway is online after successful deployment.

![](images/online.png)

`Tags: Microsoft.Resources/deployments, Microsoft.DataFactory/dataFactories/gateways, Microsoft.Network/networkSecurityGroups, Microsoft.Storage/storageAccounts, Microsoft.Network/publicIPAddresses, Microsoft.Network/networkInterfaces, Microsoft.Compute/virtualMachines, extensions, CustomScriptExtension`
