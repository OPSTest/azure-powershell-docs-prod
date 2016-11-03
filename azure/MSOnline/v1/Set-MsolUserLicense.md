---
external help file: Microsoft.Online.Administration.Automation.PSModule.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 0A3B58FA-9320-4E23-90AA-A75842492AC9
updated_at: 11/3/2016 5:22 PM
ms.date: 11/3/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/MSOnline/v1/Set-MsolUserLicense.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/cedef1609da4230592c00be27ccc62e342e2df61/Azure%20AD%20Cmdlets/MSOnline/v1/Set-MsolUserLicense.md
ms.topic: reference
ms.prod: powershell
ms.service: Azure PowerShell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Set-MsolUserLicense

## SYNOPSIS
Updates the license assignment for a user.

## SYNTAX

### SetUserLicenses__0 (Default)
```
Set-MsolUserLicense -ObjectId <Guid> [-LicenseOptions <LicenseOption[]>] [-AddLicenses <String[]>]
 [-RemoveLicenses <String[]>] [-TenantId <Guid>] [<CommonParameters>]
```

### SetUserLicensesByUpn__0
```
Set-MsolUserLicense [-LicenseOptions <LicenseOption[]>] -UserPrincipalName <String> [-AddLicenses <String[]>]
 [-RemoveLicenses <String[]>] [-TenantId <Guid>] [<CommonParameters>]
```

## DESCRIPTION
The Set-MsolUserLicense cmdlet can be used to adjust the licenses for a user.
This can include adding a new license, removing a license, updating the license options, or any combination of these actions.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Set-MsolUserLicense -UserPrincipalName user@contoso.com -AddLicenses "Contoso:ENTERPRISEPACK"

          None
```

Description

-----------

This command adds the Office 365 for enterprises license to the user.

### -------------------------- EXAMPLE 2 --------------------------
```
Set-MsolUserLicense -UserPrincipalName user@contoso.com -RemoveLicenses "contoso:ENTERPRISEPACK"

          None
```

Description

-----------

This command removes the Office 365 for enterprises license from the user. 
This may result in the user's data being removed from each service.

### -------------------------- EXAMPLE 3 --------------------------
```
Set-MsolUserLicense -UserPrincipalName user@contoso.com -AddLicenses "contoso:DESKLESS" -RemoveLicenses "contoso:ENTERPRISEPACK"

          None
```

Description

-----------

This command replaces the Office 365 for enterprises license with an Office 365 Deskless license. 
This will be done in one single operation (so the user will not end up in an intermediate state where the Office 365 for enterprises license is removed without Office 365 Deskless being added).

## PARAMETERS

### -AddLicenses
A list of licenses to assign to the user.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -LicenseOptions
Any license- or SKU-specific settings.
Used to disable individual services when assigning a license.

```yaml
Type: LicenseOption[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ObjectId
The unique ID of the user to update licenses for.

```yaml
Type: Guid
Parameter Sets: SetUserLicenses__0
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -RemoveLicenses
A list of licenses to remove from the user.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
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
The user ID of the user to update.

```yaml
Type: String
Parameter Sets: SetUserLicensesByUpn__0
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


