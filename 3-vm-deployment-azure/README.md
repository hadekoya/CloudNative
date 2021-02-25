# VM Deployments using ARM Tool

Building an ARM template for Virtual Machine deployment in Azure

## Prerequisite

- Install Azure CLI

## Execute

- Log in to the Azure Portal via CLI by using command below

`az login`

- Execute ARM template by using command below. Script requires existing resource group and admin password for the ubuntu VM

`az deployment group create --resourcegroup MYEXISTINGRESOURCEGROUP --template-file template.json -p adminPassword="MYADMINPASSWORD"`
