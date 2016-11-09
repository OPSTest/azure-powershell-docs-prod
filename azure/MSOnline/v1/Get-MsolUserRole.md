---
external help file: Microsoft.Online.Administration.Automation.PSModule.dll-Help.xml
online version:
schema: 2.0.0
ms.assetid: 13C8D948-E093-45E7-A5B5-BC38FAFCCEC7
updated_at: 11/7/2016 11:36 PM
ms.date: 11/7/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/MSOnline/v1/Get-MsolUserRole.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/6b2ae75363a4a068e37ba677387ea47a1caaeea3/Azure%20AD%20Cmdlets/MSOnline/v1/Get-MsolUserRole.md
ms.topic: reference
ms.prod: powershell
ms.service: Azure PowerShell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-MsolUserRole

## SYNOPSIS
Retrieves a list of roles that the specified user is a member of.

## SYNTAX

### ListRolesForUser__0 (Default)
```
Get-MsolUserRole -ObjectId <Guid> [-TenantId <Guid>] [<CommonParameters>]
```

### ListRolesForUserByUpn__0
```
Get-MsolUserRole -UserPrincipalName <String> [-TenantId <Guid>] [<CommonParameters>]
```

## DESCRIPTION
The Get-MsolUserRole cmdlet is used to retrieve all of the administrator roles that the specified user belongs to.
This cmdlet will also return roles that the user is a member of through security group membership.

## EXAMPLES

### Example 1:
```
PS C:\> Get-MsolUserRole -UserPrincipalName user@contoso.com

          Returns a list of roles.
```

Description

-----------

This command retrieves all groups that user@contoso.com is a member of.

## PARAMETERS

### -ObjectId
The ID of the user to retrieve roles for.

```yaml
Type: Guid
Parameter Sets: ListRolesForUser__0
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -TenantId
The unique ID of the tenant to perform the operation on.
If this is not provided then the value will default to the tenant of the current user.
This parameter is only applicable to partner users.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases:

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -UserPrincipalName
The user ID of the user to retrieve roles for.

```yaml
Type: String
Parameter Sets: ListRolesForUserByUpn__0
Aliases:

Required: True
Position: Named
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
