---
external help file: Microsoft.Azure.Commands.ResourceManager.Cmdlets.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: F3209D1C-C251-4149-AD24-D4A2CFF0D362
updated_at: 1/9/2017 9:52 PM
ms.date: 1/9/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.2.0/Register-AzureRmResourceProvider.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.2.0/Register-AzureRmResourceProvider.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4f60f66b5229674cbde5c80b99ac704ad8318378/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v3.2.0/Register-AzureRmResourceProvider.md
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

# Register-AzureRmResourceProvider

## SYNOPSIS
Registers a resource provider.

## SYNTAX

```
Register-AzureRmResourceProvider -ProviderNamespace <String> [-ApiVersion <String>] [-Pre] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
The **Register-AzureRmResourceProvider** cmdlet registers an Azure resource provider.

## EXAMPLES


## PARAMETERS

### -ProviderNamespace
Specifies the namespace of the resource provider.

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

### -ApiVersion
Specifies the API version that is supported by the resource Provider.
You can specify a different version than the default version.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
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

### -Pre
Indicates that this cmdlet considers pre-release API versions when it automatically determines which version to use.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
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

[Get-AzureRmResourceProvider](xref:ResourceManager/AzureRM.Resources/v3.2.0/Get-AzureRmResourceProvider.md)

[Unregister-AzureRmResourceProvider](xref:ResourceManager/AzureRM.Resources/v3.2.0/Unregister-AzureRmResourceProvider.md)


