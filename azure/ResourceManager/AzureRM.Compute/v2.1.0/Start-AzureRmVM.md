---
external help file: Microsoft.Azure.Commands.Compute.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 9A049236-1523-452A-97BF-1269B5B5D414
updated_at: 11/11/2016 11:03 PM
ms.date: 11/11/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.1.0/Start-AzureRmVM.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.1.0/Start-AzureRmVM.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/79eeb985ea480979357fb4695832a0c3d29a48bf/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.1.0/Start-AzureRmVM.md
ms.topic: reference
ms.prod: powershell
ms.technology: Azure PowerShell
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: False
ms.service: azure-powershell
---

# Start-AzureRmVM

## SYNOPSIS
Starts an Azure virtual machine.

## SYNTAX

### ResourceGroupNameParameterSetName (Default)
```
Start-AzureRmVM [-Name] <String> [-ResourceGroupName] <String> [<CommonParameters>]
```

### IdParameterSetName
```
Start-AzureRmVM [-Name] <String> [-Id] <String> [<CommonParameters>]
```

## DESCRIPTION
The **Start-AzureRmVM** cmdlet starts an Azure virtual machine.

## EXAMPLES

### Example 1: Start a virtual machine
```
PS C:\>Start-AzureRmVM -ResourceGroupName "ResourceGroup11" -Name "VirtualMachine07"
```

This command starts the virtual machine named VirtualMachine07 in ResourceGroup11.

## PARAMETERS

### -Id
Specifies the Resource ID of the virtual machine.

```yaml
Type: String
Parameter Sets: IdParameterSetName
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the name of the virtual machine to start.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group of the virtual machine.

```yaml
Type: String
Parameter Sets: ResourceGroupNameParameterSetName
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmVM](xref:ResourceManager/AzureRM.Compute/v2.1.0/Get-AzureRmVM.md)

[New-AzureRmVM](xref:ResourceManager/AzureRM.Compute/v2.1.0/New-AzureRmVM.md)

[Remove-AzureRmVM](xref:ResourceManager/AzureRM.Compute/v2.1.0/Remove-AzureRmVM.md)

[Restart-AzureRmVM](xref:ResourceManager/AzureRM.Compute/v2.1.0/Restart-AzureRmVM.md)

[Stop-AzureRmVM](xref:ResourceManager/AzureRM.Compute/v2.1.0/Stop-AzureRmVM.md)

[Update-AzureRmVM](xref:ResourceManager/AzureRM.Compute/v2.1.0/Update-AzureRmVM.md)


