# Azure PowerShell Starter Commands

## Authentication

```powershell
Connect-AzAccount
Get-AzContext
Get-AzSubscription
Set-AzContext -Subscription "<YOUR_SUBSCRIPTION_ID>"
```

## Resource groups

```powershell
Get-AzResourceGroup
Get-AzResourceGroup -Name "<YOUR_RESOURCE_GROUP>"
```

## Resources

```powershell
Get-AzResource -ResourceGroupName "<YOUR_RESOURCE_GROUP>"
```

## Virtual machines

```powershell
Get-AzVM
Get-AzVM -ResourceGroupName "<YOUR_RESOURCE_GROUP>"
Get-AzVM -ResourceGroupName "<YOUR_RESOURCE_GROUP>" -Status
```

> Treat this as a practice starter. Record only commands that you actually understand and validate.
