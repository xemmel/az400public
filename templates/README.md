


## From Powershell deploy a template


```powershell

$rgName = "ffff-rg";

### Create Resource Group
az group create --name $rgName --location westeurope;


### Deploy template (arm/json bicep/bicep)
az deployment group create --resource-group $rgName --template-file ./sub/fdfdf.json

```