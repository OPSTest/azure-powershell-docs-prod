---
external help file: Microsoft.Online.Administration.Automation.PSModule.dll-Help.xml
online version:
schema: 2.0.0
ms.assetid: 5EFA8894-F622-48D0-97D4-3D673E08FF37
updated_at: 11/10/2016 4:53 PM
ms.date: 11/10/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/MSOnline/v1/Set-MsolCompanySecurityComplianceContactInformation.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/fa0df7d7c5fc79297507723a62f5fc4575dafc5e/Azure%20AD%20Cmdlets/MSOnline/v1/Set-MsolCompanySecurityComplianceContactInformation.md
ms.topic: reference
ms.prod: powershell
ms.service: Azure PowerShell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Set-MsolCompanySecurityComplianceContactInformation

## SYNOPSIS
Sets company-level security and compliance contact preferences.

## SYNTAX

```
Set-MsolCompanySecurityComplianceContactInformation [-SecurityComplianceNotificationEmails <String[]>]
 [-SecurityComplianceNotificationPhones <String[]>] [-TenantId <Guid>] [<CommonParameters>]
```

## DESCRIPTION
The **Set-MsolCompanySecurityComplianceContactInformation** cmdlet sets company-level security and compliance contact preferences.
These preferences include email addresses and phone numbers of the tenant’s security and compliance contacts.
The contact is used for notification purposes.


## EXAMPLES

### Example 1:
```
Set-MsolCompanySecurityComplianceContactInformation -SecurityComplianceNotificationEmails "EvanNarvaez@contoso.com", "ElisaDaugherty@contoso.com" -SecuritComplianceNotificationPhones "555-555-0012","555-555-0199"
```

This command sets multiple email addresses as company-level security and compliance contacts and respective phone numbers for each contact.


## PARAMETERS

### -SecurityComplianceNotificationEmails
Specifies an array of company-level security and compliance contact email addresses.

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

### -SecurityComplianceNotificationPhones
Specifies an array of company-level security and compliance contact phone numbers.

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
Specifies the unique ID of the tenant on which to perform the operation.
The default value is the tenant of the current user.
This parameter applies only to partner users.


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

### System.String[]
System.Nullable`1[[System.Guid, mscorlib, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089]]

## OUTPUTS

### System.Object

## NOTES

## RELATED LINKS
