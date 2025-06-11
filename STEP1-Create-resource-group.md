#### PowerShell and Bash just differ in variable declaration; 
#### In PowerShell you add a $ before variable, in Bash you don't;
#### Whether in Windows or Ubuntu, after installing the [PowerShell module](https://learn.microsoft.com/en-us/powershell/scripting/install/installing-powershell?view=powershell-7.5), you can execute the commands in bash or cmd and stricly running in PowerShell Prompt is not needed;
#### Another deifference is line split.
#### In powershell you split a line using ` (Backtick)
#### In BASH you split a line using \       (Backslash)
---

## Using AZCLI Module
### **Connect to Azure**
```bash
az login
```
### **Declare Variables in PowerShell**
```PowerShell
$ResourceGroup = "myResourceGroup"
```
OR
### **Declare Variables in BASH ($ at beginning not needed)**
```bash
ResourceGroup = "myResourceGroup"
```
### **Create a resource group**
```bash
az group create --name $ResourceGroup --location $Location
```
---
