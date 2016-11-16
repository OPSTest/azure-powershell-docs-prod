---
external help file: SMAzure_Compute.xml
online version: 
schema: 2.0.0
updated_at: 8/26/2016 9:24 PM
ms.date: 8/26/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/Service%20Management/Compute%20Cmdlets/v0.9.8/Add-AzureVMNetworkInterface.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/1457b00e4be43f52e047ac6fd4ed87f3565c5548/azureps-cmdlets-docs/Service%20Management/Compute%20Cmdlets/v0.9.8/Add-AzureVMNetworkInterface.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: 
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Add-AzureVMNetworkInterface
## SYNOPSIS
Add a Network Interface to the VM

## SYNTAX

```
Add-AzureVMNetworkInterface [-VM] <PSVirtualMachine> [-Id] <String> [-Profile <AzureProfile>]
```

## DESCRIPTION
This cmdlets allows you to add a NIC to the VM at creation time or to an existing VM

## EXAMPLES

### --------------------------  Add a Network Interface to a new VM  --------------------------
```
PS C:\> # Get the VM
          $vm = Get-AzureVM -ResourceGroupName "myRG" -Name "crpVM

          # Add a Network Interface to the VM
          Add-AzureVMNetworkInterface ?VM $vm ?Id "/subscriptions/subscriptionId/resourceGroups/resourceGroupName/providers/Microsoft.Network/NetworkAdapters/Nic1"
```

### --------------------------  Add a Network Interface to an existing VM  --------------------------
```
PS C:\> # Get the VM
          $vm = Get-AzureVM -ResourceGroupName "myRG" -Name "crpVM"

          # Add a Network Interface to the VM
          Add-AzureVMNetworkInterface ?VM $vm ?Id "/subscriptions/subscriptionId/resourceGroups/resourceGroupName/providers/Microsoft.Network/NetworkAdapters/Nic1"

          # Update VM state
          Update-AzureVM -ResourceGroupName "myRG" -Name "crpVM" ?VM $vm
```

## PARAMETERS

### -Id
Id of the Network Interface.
This can be gotten using the Get-AzureNetworkInterface cmdlet.

```yaml
Type: String
Parameter Sets: (All)
Aliases: NicId,NetworkInterfaceId

Required: True
Position: 2
Default value: None
Accept pipeline input: True(ByPropertyName)
Accept wildcard characters: False
```

### -Profile
```yaml
Type: AzureProfile
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -VM
Local VM Object to add the Network Interface to.
The local VM object can be created with New-AzureVMConfig cmdlet or gotten through the Get-AzureVM cmdlet.

```yaml
Type: PSVirtualMachine
Parameter Sets: (All)
Aliases: VMProfile

Required: True
Position: 1
Default value: None
Accept pipeline input: True(ByValue,ByPropertyName)
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
