---
external help file: azuread.help.xml
online version: 
schema: 2.0.0
updated_at: 12/2/2016 6:50 PM
ms.date: 12/2/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2/Remove-AzureADMSGroup.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2/Remove-AzureADMSGroup.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/9d73de920ad3690865797cee4594d4633c9b692d/Azure%20AD%20Cmdlets/AzureAD/v2/Remove-AzureADMSGroup.md
ms.topic: reference
ms.technology: Azure PowerShell
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: carolz
open_to_public_contributors: true
ms.service: active-directory
---

# Remove-AzureADMSGroup

## SYNOPSIS
Removes an Azure AD group.

## SYNTAX

```
Remove-AzureADMSGroup [-Id <String>]
```

## DESCRIPTION
The **Remove-AzureADMSGroup** cmdlet removes an Azure Active Directory (Azure AD) group.

## EXAMPLES

### Example 1: Remove a group
```
PS C:\> Remove-AzureADMSGroup -Id "ce0a2213-bd57-4e2f-b9fa-408582e2e260"
```

This cmdlet removes the group that has the specified ID.

## PARAMETERS

### -Id
Specifies the ID of the group that this cmdlet removes.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

## INPUTS

### System.String

## OUTPUTS

### System.Object

## NOTES
This cmdlet is currently in Public Preview.
While a cmdlet is in Public Preview, we may make changes to the cmdlet which could have unexpected effects.
We recommend that you do not use this cmdlet in a production environment.

## RELATED LINKS
[Get-AzureADMSGroup](xref:AzureAD/v2/Get-AzureADMSGroup.md)

[New-AzureADMSGroup](xref:AzureAD/v2/New-AzureADMSGroup.md)

[Set-AzureADMSGroup](xref:AzureAD/v2/Set-AzureADMSGroup.md)

[Using attributes to create advanced rules](https://azure.microsoft.com/en-us/documentation/articles/active-directory-accessmanagement-groups-with-advanced-rules/)
