---
external help file: SMAzure_Compute.xml
online version: 
schema: 2.0.0
updated_at: 8/26/2016 9:24 PM
ms.date: 8/26/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/Service%20Management/Compute%20Cmdlets/v1.0/Show-AzurePortal.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/1457b00e4be43f52e047ac6fd4ed87f3565c5548/azureps-cmdlets-docs/Service%20Management/Compute%20Cmdlets/v1.0/Show-AzurePortal.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: 
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Show-AzurePortal
## SYNOPSIS
Show the Azure Management Portal.

## SYNTAX

```
Show-AzurePortal [[-Name] <String>] [-Realm <String>]
```

## DESCRIPTION
This topic describes the cmdlet in the 0.8.10 version of the Microsoft Azure PowerShell module.
To get the version of the module you're using, in the Azure PowerShell console, type (Get-Module -Name Azure).Version.

The Show-AzurePortal cmdlet shows the Azure Management Portal.

## EXAMPLES

### 1:
```
PS C:\>Show-AzurePortal -Name mySite
```

This example opens a browser on the Azure portal, showing information about a website named 'mySite'.

## PARAMETERS

### -Name
Specifies the name of the website to show in the portal.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Realm
Specifies the organization ID to use for federated authentication when displaying the Azure Portal.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: 
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Show-AzureWebsite](3b828275-d62a-4c04-9767-15d6f743557c)

