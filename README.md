# Azure CLI Cheatsheet

## Create an Azure Container Registry
```
az acr create --resource-group myapp-rg --name mycontainerregistry --sku Basic
```

## Build container image
```
az acr build --registry $ACR_NAME --image helloacrtasks:v1 .
```

## Replicate region for an ACR
```
az acr replication create --registry $ACR_NAME --location japaneast
```
