---
external help file: Microsoft.Azure.Commands.ApiManagement.ServiceManagement.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: D6B7F253-03CD-40BE-87D6-E4AE300A29D5
updated_at: 11/3/2016 10:58 PM
ms.date: 11/3/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/v3.0.0/Remove-AzureRmApiManagementProduct.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/b0dc3fda3721a600f2fff31599b45845d71f44f4/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/v3.0.0/Remove-AzureRmApiManagementProduct.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Remove-AzureRmApiManagementProduct

## SYNOPSIS
Removes an existing API Management product.

## SYNTAX

```
Remove-AzureRmApiManagementProduct -Context <PsApiManagementContext> -ProductId <String> [-DeleteSubscriptions]
 [-PassThru] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRmApiManagementProduct** cmdlet removes an existing API Management product.

## EXAMPLES

### Example 1: Remove an existing product and all subscriptions
```
PS C:\>Remove-AzureRmApiManagementProduct -Context $APImContext -Id "0123456789" -DeleteSubscriptions -Force
```

This command removes an existing product and all subscriptions.

## PARAMETERS

### -Context
Specifies an instance of the **PsApiManagementContext** object.

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

### -ProductId
Specifies the identifier of the existing product.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -DeleteSubscriptions
Indicates whether to delete subscriptions to the product.
If you do not set this parameter and subscriptions exists, an exception is thrown.

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

### -PassThru
Indicates that this cmdlet returns a value of $True, if it succeeds, or a value of $False, if it fails.

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

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.Shows what would happen if the cmdlet runs.
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

### -Confirm
Prompts you for confirmation before running the cmdlet.Prompts you for confirmation before running the cmdlet.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### bool

## NOTES

## RELATED LINKS

[Get-AzureRmApiManagementProduct](xref:ResourceManager/AzureRM.ApiManagement/v3.0.0/Get-AzureRmApiManagementProduct.md)

[New-AzureRmApiManagementProduct](xref:ResourceManager/AzureRM.ApiManagement/v3.0.0/New-AzureRmApiManagementProduct.md)

[Set-AzureRmApiManagementProduct](xref:ResourceManager/AzureRM.ApiManagement/v3.0.0/Set-AzureRmApiManagementProduct.md)

