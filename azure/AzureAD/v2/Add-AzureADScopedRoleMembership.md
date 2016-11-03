---
external help file: Microsoft.Open.AzureADBeta.Graph.PowerShell.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: B505822C-4BAA-4EC5-BB0A-128C093930C6
updated_at: 11/3/2016 8:54 PM
ms.date: 11/3/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2/Add-AzureADScopedRoleMembership.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/ded621ecc7ac929eccefd449f9b60e77f303f3e1/Azure%20AD%20Cmdlets/AzureAD/v2/Add-AzureADScopedRoleMembership.md
ms.topic: reference
ms.prod: powershell
ms.service: Azure PowerShell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Add-AzureADScopedRoleMembership

## SYNOPSIS
Adds a scoped role membership to an administrative unit.

## SYNTAX

```
Add-AzureADScopedRoleMembership -ObjectId <String> [-AdministrativeUnitObjectId <String>]
 [-RoleObjectId <String>] [-RoleMemberInfo <RoleMemberInfo>] [<CommonParameters>]
```

## DESCRIPTION
The **Add-AzureADScopedRoleMembership** cmdlet adds a scoped role membership to an administrative unit.

## PARAMETERS

### -AdministrativeUnitObjectId
Specifies the ID of an admininstrative unit.

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

### -ObjectId


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

### -RoleMemberInfo
Specifies a **RoleMemberInfo** object. 
```yaml
Type: RoleMemberInfo
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RoleObjectId
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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
[Get-AzureADScopedRoleMembership](./Get-AzureADScopedRoleMembership)

[Remove-AzureADScopedRoleMembership](./Remove-AzureADScopedRoleMembership)

