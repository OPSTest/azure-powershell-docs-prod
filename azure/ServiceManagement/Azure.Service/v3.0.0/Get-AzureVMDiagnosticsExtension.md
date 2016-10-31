---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: 87fe577f-4470-4790-818d-5e77007dd965
schema: 2.0.0
ms.assetid: DD8DBD57-462F-426F-A03F-E6BAC629D0D3
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v3.0.0/Get-AzureVMDiagnosticsExtension.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v3.0.0/Get-AzureVMDiagnosticsExtension.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureVMDiagnosticsExtension

## SYNOPSIS
Gets the settings of the Azure Diagnostics extension on a virtual machine.

## SYNTAX

```
Get-AzureVMDiagnosticsExtension -VM <IPersistentVM> [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureVMDiagnosticsExtension** cmdlet gets the settings of the Microsoft Azure Diagnostics extension on a virtual machine.

## EXAMPLES

### Example 1: Get the diagnostics extension applied to a virtual machine
```
PS C:\>Get-AzureVMDiagnosticsExtension -VM $VM
```

This command gets the diagnostics extension applied to the specified virtual machine as stored in the variable $VM.

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
Type: AzureSMProfile
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

[Remove-AzureVMDiagnosticsExtension](xref:ServiceManagement/Azure.Service/v3.0.0/Remove-AzureVMDiagnosticsExtension.md)

[Set-AzureVMDiagnosticsExtension](xref:ServiceManagement/Azure.Service/v3.0.0/Set-AzureVMDiagnosticsExtension.md)


