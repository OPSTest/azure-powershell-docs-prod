---
external help file: Microsoft.Azure.Commands.Compute.dll-Help.xml
ms.assetid: D83F9C13-283E-444D-8CBE-7B0B8769B809
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.3.0/Update-AzureRmVmss.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.3.0/Update-AzureRmVmss.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: ResourceManager_AzureRM_Compute_v2_3_0_Update_AzureRmVmss_md
---

# Update-AzureRmVmss

## SYNOPSIS
Updates the state of a VMSS.

## SYNTAX

```
Update-AzureRmVmss [-WhatIf] [-Confirm] [-ResourceGroupName] <String> [-Name] <String>
 [-VirtualMachineScaleSet] <VirtualMachineScaleSet> [<CommonParameters>]
```

## DESCRIPTION
The **Update-AzureRmVmss** cmdlet updates the state of a Virtual Machine Scale Set (VMSS) to the state of a local VMSS object.

## EXAMPLES

### Example 1: Update the state of a VMSS to the state of a local VMSS object.
```
PS C:\>Update-AzureRmVmss -ResourceGroupName "Group001" -Name "VMSS001" -VirtualMachineScaleSet "LocalVMSS"
```

This command updates the state of the VMSS named VMSS001 that belongs to the resource group named Group001 to the state of a local VMSS object named LocalVMSS.

## PARAMETERS

### -Name
Specifies the name of the VMSS that this cmdlet updates the state for.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group the VMSS belongs to.

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

### -VirtualMachineScaleSet
Specifies a local VMSS object.
To obtain a VMSS object, use the Get-AzureRmVmss cmdlet.
This virtual machine object contains the updated state for the VMSS.

```yaml
Type: VirtualMachineScaleSet
Parameter Sets: (All)
Aliases: 

Required: True
Position: 4
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.

The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmVmss](xref:ResourceManager/AzureRM.Compute/v2.3.0/Get-AzureRmVmss.md)

[New-AzureRmVmss](xref:ResourceManager/AzureRM.Compute/v2.3.0/New-AzureRmVmss.md)

[Remove-AzureRmVmss](xref:ResourceManager/AzureRM.Compute/v2.3.0/Remove-AzureRmVmss.md)

[Restart-AzureRmVmss](xref:ResourceManager/AzureRM.Compute/v2.3.0/Restart-AzureRmVmss.md)

[Set-AzureRmVmss](xref:ResourceManager/AzureRM.Compute/v2.3.0/Set-AzureRmVmss.md)

[Start-AzureRmVmss](xref:ResourceManager/AzureRM.Compute/v2.3.0/Start-AzureRmVmss.md)

[Stop-AzureRmVmss](xref:ResourceManager/AzureRM.Compute/v2.3.0/Stop-AzureRmVmss.md)


