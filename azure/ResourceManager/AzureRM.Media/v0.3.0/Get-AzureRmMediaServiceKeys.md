---
external help file: Microsoft.Azure.Commands.Media.dll-Help.xml
online version: 54d094dc-043b-4d25-93d4-2f4ffe8d7081
schema: 2.0.0
ms.assetid: CF44604E-FD17-4E09-AEAA-50DE32CD55EC
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Media/v0.3.0/Get-AzureRmMediaServiceKeys.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Media/v0.3.0/Get-AzureRmMediaServiceKeys.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: PowerShellHelpPub
---

# Get-AzureRmMediaServiceKeys

## SYNOPSIS
Gets key information for accessing the REST endpoint associated with the media service.

## SYNTAX

```
Get-AzureRmMediaServiceKeys [-ResourceGroupName] <String> [-AccountName] <String> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmMediaServiceKeys** cmdlet gets key information for accessing the Representational State Transfer (REST) endpoint associated with the Azure media service.

## EXAMPLES

### Example 1: Get the key information for accessing the media service
```
PS C:\>Get-AzureRmMediaServiceKeys -ResourceGroupName "ResourceGroup001" -AccountName "MediaService001"
```

This command gets the key information for accessing the media service named MediaService001 that belongs to the resource group named ResourceGroup001.

## PARAMETERS

### -ResourceGroupName
Specifies the name of the resource group that contains the media service.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -AccountName
Specifies the name of the media service that this cmdlet gets the media service keys from.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Name, ResourceName

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

[Set-AzureRmMediaServiceKey](./Set-AzureRmMediaServiceKey.md)


