---
external help file: Microsoft.Azure.Commands.ApiManagement.ServiceManagement.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 3B5FC8E3-5A02-4F3B-81F0-51DFE47A201B
updated_at: 11/3/2016 10:58 PM
ms.date: 11/3/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/v3.0.0/Set-AzureRmApiManagementTenantAccess.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/b0dc3fda3721a600f2fff31599b45845d71f44f4/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/v3.0.0/Set-AzureRmApiManagementTenantAccess.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Set-AzureRmApiManagementTenantAccess

## SYNOPSIS
Enables or disables tenant access.

## SYNTAX

```
Set-AzureRmApiManagementTenantAccess -Context <PsApiManagementContext> -Enabled <Boolean> [-PassThru]
 [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureRmApiManagementTenantAccess** cmdlet enables or disables tenant access.

## EXAMPLES

### Example 1: Enable tenant access
```
PS C:\>Set-AzureRmApiManagementTenantAccess -Context $ApimContext -Enabled $True
```

This command enables tenant access in the specified context.

## PARAMETERS

### -Context
Specifies a **PsApiManagementContext** object.

```yaml
Type: PsApiManagementContext
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Enabled
Specifies whether this cmdlet enables or disables tenant access.
Specify a value of $True to enable or $False to disable.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Indicates that this cmdlet returns the **PsApiManagementAccessInformation** that this cmdlet modifies.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.Azure.Commands.ApiManagement.ServiceManagement.Models.PsApiManagementAccessInformation

## NOTES

## RELATED LINKS

[Get-AzureRmApiManagementTenantAccess](xref:ResourceManager/AzureRM.ApiManagement/v3.0.0/Get-AzureRmApiManagementTenantAccess.md)

