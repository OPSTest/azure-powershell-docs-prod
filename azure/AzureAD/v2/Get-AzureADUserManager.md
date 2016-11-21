---
external help file: azuread.help.xml
online version: 
schema: 2.0.0
updated_at: 11/21/2016 8:09 PM
ms.date: 11/21/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2/Get-AzureADUserManager.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/e79870303c4a5b18f88c61a5fe206bd45af8c480/Azure%20AD%20Cmdlets/AzureAD/v2/Get-AzureADUserManager.md
ms.topic: reference
ms.prod: 
ms.service: active-directory
ms.technology: Azure PowerShell
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: carolz
id: AzureAD_v2_Get_AzureADUserManager_md
---

# Get-AzureADUserManager

## SYNOPSIS
Retrieves the manager of a user from Azure Active Directory

## SYNTAX

```
Get-AzureADUserManager -ObjectId <String>
```

## DESCRIPTION

## EXAMPLES

### Retrieve the manager of a given user
```
$UserId = (Get-AzureADUser -Top 1).ObjectId
Get-AzureADUserManager -ObjectId $UserId

Output:


ObjectId                             ObjectType 
--------                             ---------- 
5e8b0f4d-2cd4-4e17-9467-b0f6a5c0c4d0 User
```

## PARAMETERS

### -ObjectId
The unique identifier of a user in Azure Active Directory (UPN or ObjectId)

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue, ByPropertyName)
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

