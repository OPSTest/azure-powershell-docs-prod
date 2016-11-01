---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 29F4ADFD-BE44-40E2-A459-CDBB6E011CD4
updated_at: 11/1/2016 10:24 PM
ms.date: 11/1/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v0.9.8/Remove-AzureVMCustomScriptExtension.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/f59f3ef60bc592383812213e69fd77ba950759ed/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v0.9.8/Remove-AzureVMCustomScriptExtension.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Remove-AzureVMCustomScriptExtension

## SYNOPSIS
Removes the custom script extension from a virtual machine.

## SYNTAX

```
Remove-AzureVMCustomScriptExtension -VM <IPersistentVM> [-Profile <AzureProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureVMCustomScriptExtension** cmdlet removes the custom script extension from a virtual machine.

## EXAMPLES

### Example 1: Remove a virtual machine custom script extension
```
PS C:\> Remove-AzureVMCustomScriptExtension -VM $VM;
```

This command removes the Azure virtual machine custom script extension from the specified virtual machine as stored in the variable $VM.

## PARAMETERS

### -VM
Specifies the persistent virtual machine object.

```yaml
Type: IPersistentVM
Parameter Sets: (All)
Aliases: InputObject

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Profile
Specifies the Azure profile from which this cmdlet reads.
If you do not specify a profile, this cmdlet reads from the local default profile.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureVMCustomScriptExtension](xref:ServiceManagement/Azure.Service/v0.9.8/Get-AzureVMCustomScriptExtension.md)

[Set-AzureVMCustomScriptExtension](xref:ServiceManagement/Azure.Service/v0.9.8/Set-AzureVMCustomScriptExtension.md)

[Azure Service Cmdlets](xref:ServiceManagement/Azure.Service/v0.9.8/Azure.Service.md)


