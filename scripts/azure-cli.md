# Azure CLI Starter Commands

## Authentication

```bash
az login
az account show
az account list --output table
az account set --subscription "<YOUR_SUBSCRIPTION_ID>"
```

## Resource groups

```bash
az group list --output table
az group show --name "<YOUR_RESOURCE_GROUP>"
```

## Resources

```bash
az resource list --resource-group "<YOUR_RESOURCE_GROUP>" --output table
```

## Virtual machines

```bash
az vm list --output table
az vm show --resource-group "<YOUR_RESOURCE_GROUP>" --name "<YOUR_VM>"
az vm show --resource-group "<YOUR_RESOURCE_GROUP>" --name "<YOUR_VM>" --show-details --output table
```

## Networking

```bash
az network vnet list --output table
az network nsg list --output table
```

## Storage

```bash
az storage account list --output table
```

> Treat this as a practice starter. Record only commands that you actually understand and validate.
