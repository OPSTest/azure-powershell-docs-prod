---
external help file: azuread.help.xml
online version: 
schema: 2.0.0
updated_at: 11/21/2016 8:09 PM
ms.date: 11/21/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2/Get-AzureADUserOwnedObject.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/e79870303c4a5b18f88c61a5fe206bd45af8c480/Azure%20AD%20Cmdlets/AzureAD/v2/Get-AzureADUserOwnedObject.md
ms.topic: reference
ms.technology: Azure PowerShell
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: carolz
open_to_public_contributors: True
ms.service: active-directory
---

# Get-AzureADUserOwnedObject

## SYNOPSIS
Get objects owned by the user.

## SYNTAX

```
Get-AzureADUserOwnedObject -ObjectId <String> [-Top <Nullable`1[Int32]>]
```

## DESCRIPTION

## EXAMPLES

### Retrieve the objects that are owned by a given user
```
$UserId = (Get-AzureADUser -Top 1).ObjectId
Get-AzureADUserOwnedObject -ObjectId $UserId
Output:

ObjectId                             ObjectType
--------                             ----------
9c2564d6-e4d7-4167-a79f-4b961512f232 Group
36db8aaf-022a-448d-aedc-34ef2ceb943c Group
529b48fb-6324-4899-88ab-fb9bd9ed0fd4 Group
0e6cf869-82ca-4647-b330-420b9a6f8ef7 Group
78045c26-218e-46fb-94b6-1a47320da153 Group
4c0ed9b7-cca2-4bb2-a2f1-736bb263ea0b Group
49a8bc01-2751-450b-a2e8-b4267f609513 Application
a0dada57-89ef-4db8-9e5f-46cca3bf2398 Group
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

### -Top
The maximum number of records to return.
If no value is provided, 100 records are returned

```yaml
Type: Nullable`1[Int32]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue, ByPropertyName)
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

