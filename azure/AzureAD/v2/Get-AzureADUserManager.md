---
external help file: Microsoft.Open.AzureAD16.Graph.PowerShell.dll-Help.xml
ms.assetid: C27027E1-A314-4EF2-82F2-396524334B99
online version: 
schema: 2.0.0
updated_at: 11/19/2016 5:55 PM
ms.date: 11/19/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2/Get-AzureADUserManager.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/78576a00e7eab32d13180fb832c5e222accdc9ce/Azure%20AD%20Cmdlets/AzureAD/v2/Get-AzureADUserManager.md
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
Gets the manager of a user.

## SYNTAX

```
Get-AzureADUserManager -ObjectId <String> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureADUserManager** cmdlet gets the manager of a user in Azure Active Directory (AD).

## EXAMPLES

### Example 1: Get the manager of a user
```
PS C:\>Get-AzureADUserManager -ObjectId "df19e8e6-2ad7-453e-87f5-037f6529ae16"

ObjectId                             ObjectType
--------                             ----------
5e8b0f4d-2cd4-4e17-9467-b0f6a5c0c4d0 User
```

This command gets the manager of the specified user.

## PARAMETERS

### -InformationAction
Specifies how this cmdlet responds to an information event. The acceptable values for this parameter are:

- Continue
- Ignore
- Inquire
- SilentlyContinue
- Stop
- Suspend

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
Specifies an information variable.

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ObjectId
The unique identifier of a user in Azure Active Directory (UPN or ObjectId)

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Remove-AzureADUserManager](xref:AzureAD/v2/Remove-AzureADUserManager.md)

[Set-AzureADUserManager](xref:AzureAD/v2/Set-AzureADUserManager.md)

