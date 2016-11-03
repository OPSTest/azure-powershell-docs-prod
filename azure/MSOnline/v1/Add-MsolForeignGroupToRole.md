---
external help file: Microsoft.Online.Administration.Automation.PSModule.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: B5D447B0-4C83-42D7-8162-1E95AF02EDA2
updated_at: 11/3/2016 5:22 PM
ms.date: 11/3/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/MSOnline/v1/Add-MsolForeignGroupToRole.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/cedef1609da4230592c00be27ccc62e342e2df61/Azure%20AD%20Cmdlets/MSOnline/v1/Add-MsolForeignGroupToRole.md
ms.topic: reference
ms.prod: powershell
ms.service: Azure PowerShell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Add-MsolForeignGroupToRole

## SYNOPSIS
Adds the specified group from a partner tenant to a Role in this tenant.

## SYNTAX

```
Add-MsolForeignGroupToRole -ForeignGroupObjectId <Guid> -ForeignCompanyObjectId <Guid> -RoleObjectId <Guid>
 [-TenantId <Guid>] [<CommonParameters>]
```

## DESCRIPTION
The Add-MsolForeignGroupToRole cmdlet is used to add a security group from a partner tenant to the specified role in this tenant.

## PARAMETERS

### -ForeignCompanyObjectId
The object ID of the partner tenant that contains the group to add.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ForeignGroupObjectId
The object ID of the group in the partner tenant to add.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -RoleObjectId
The object ID of the role to add the group to.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -TenantId
The unique ID of the tenant to perform the operation on. 
If this is not provided then it will default to the tenant of the current user. 
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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS


