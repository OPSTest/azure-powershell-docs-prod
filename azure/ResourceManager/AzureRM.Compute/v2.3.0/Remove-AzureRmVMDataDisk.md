---
external help file: Microsoft.Azure.Commands.Compute.dll-Help.xml
ms.assetid: 4538ECE1-A0B6-4439-B931-73E11B83D72A
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.3.0/Remove-AzureRmVMDataDisk.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.3.0/Remove-AzureRmVMDataDisk.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Remove-AzureRmVMDataDisk

## SYNOPSIS
Removes a data disk from a virtual machine.

## SYNTAX

```
Remove-AzureRmVMDataDisk [-VM] <PSVirtualMachine> [-DataDiskNames] <String[]> [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRmVMDataDisk** cmdlet removes a data disk from a virtual machine.

## EXAMPLES

### Example 1: Remove a data disk from a virtual machine
```
PS C:\>$VirtualMachine = Get-AzureRmVM -ResourceGroupName "ResourceGroup11" -Name "VirtualMachine07" 
PS C:\> Remove-AzureRmVMDataDisk -VM $VirtualMachine -Name "Disk3"
PS C:\> Update-AzureRmVM -ResourceGroupName "ResourceGroup11" -Name "VirtualMachine07" -VM $VirtualMachine
```

The first command gets the virtual machine named VirtualMachine07 by using the **Get-AzureRmVM** cmdlet.
The command stores the virtual machine in the $VirtualMachine variable.

The second command removes the data disk named Disk3 from the virtual machine stored in $VirtualMachine.

The final command updates the state of the virtual machine stored in $VirtualMachine in ResourceGroup11.

## PARAMETERS

### -DataDiskNames
Specifies the names of one or more data disks that this cmdlet removes.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: Name

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -VM
Specifies the local virtual machine object from which to remove a data disk.
To obtain a virtual machine object, use the Get-AzureRmVM cmdlet.

```yaml
Type: PSVirtualMachine
Parameter Sets: (All)
Aliases: VMProfile

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Add-AzureRmVMDataDisk](xref:ResourceManager/AzureRM.Compute/v2.3.0/Add-AzureRmVMDataDisk.md)

[Get-AzureRmVM](xref:ResourceManager/AzureRM.Compute/v2.3.0/Get-AzureRmVM.md)


