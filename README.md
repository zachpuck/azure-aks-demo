# Azure AKS demo templates
Azure Resource Manager (ARM) templates

deploy using [az cli](https://docs.microsoft.com/en-us/cli/azure/?view=azure-cli-latest)

az login
az account set --subscription "subscriptionId"

list available locations: `az account list-locations`


Apply ARM template:
```
az group deployment create \
    --resource-group "demo-aks" \
    --name "demo-aks-cluster" \
    --parameters "./demo-parameters.json" \
    --template-file "./template.json"
```
[documentation reference](https://docs.microsoft.com/en-us/cli/azure/group/deployment?view=azure-cli-latest#az-group-deployment-create)