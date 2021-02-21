# Automating Azure using Powershell

Objective to create resource groups using powershell

## Pre-requisite

- Powershell
  `brew install --cask powershell`
- Azure CLI
  `brew update && brew install azure-cli`
  `az login`
- [Azure PowerShell module](https://docs.microsoft.com/en-us/powershell/azure/install-az-ps?view=azps-5.5.0#code-try-3)

```powershell
Install the Azure PowerShell module

if ($PSVersionTable.PSEdition -eq 'Desktop' -and (Get-Module -Name AzureRM -ListAvailable)) {
Write-Warning -Message ('Az module not installed. Having both the AzureRM and ' +
'Az modules installed at the same time is not supported.')
} else {
Install-Module -Name Az -AllowClobber -Scope CurrentUser
}
```

- Connect AZ powershell to Azure  
  `Connect-AzAccount`

## Execution

New-ResourceGroup -rgName sampleresouregroup -location eastus2

## Linting
