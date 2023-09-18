



### Set git config

```powershell

git config --global alias.xlist 'log --graph --all --oneline --decorate'
git config --global alias.add-commit '!git add -A && git commit'

  git config --global user.email "..."
  git config --global user.name "...."

```


### Powershell / Cli commands


```powershell

### Logon CLI
az login --use-device-code

### Logon Powershell
Login-AzAccount -UseDeviceAuthentication

### Change Subscription
az account set -s subid
Set-AzContext -SubscriptionId 9bc198aa-089c-4698-a7ef-8af058b48d90

### List Resource Group
az group list --output table
Get-AzResourceGroup

### Select Specific Resource Groups (not westeurope) to gridview -> Delete selected resource groups
Get-AzResourceGroup | Where-Object {$_.Location -ne "westeurope"} | Out-GridView -PassThru | Remove-AzResourceGroup -Force -AsJob



```