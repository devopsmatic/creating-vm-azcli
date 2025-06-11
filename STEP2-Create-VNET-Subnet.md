### Using AZCLI and BASH
### **Delete the variables declared in STEP1 for better practice and recreate again
```bash
az group delete --name $ResourceGroup --yes --no-wait
```
**Wait for a minute or so**
---
### Declare Resource group Variables
```bash
ResourceGroup = "myResourceGroup"
Location = "East US"
```
### Declare VNET and Subnet variables
```bash
$VNetName = "myVNet"
$VNetAddressSpace = "10.0.0.0/16"
$SubnetName = "mySubnet"
$SubnetAddressSpace = "10.0.0.0/24"
```
### Create VNET and Subnet
```bash
az network vnet create \
  --resource-group $ResourceGroup \
  --name "${VMName}VNet" \
  --address-prefix 10.0.0.0/16 \
  --subnet-name "${VMName}Subnet" \
  --subnet-prefix 10.0.0.0/24 \
  --location $Location
```
