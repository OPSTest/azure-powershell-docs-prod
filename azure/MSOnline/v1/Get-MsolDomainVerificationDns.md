---
external help file: Microsoft.Online.Administration.Automation.PSModule.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 20D3AFFB-C7B5-40C4-8379-CE115EC668FC
updated_at: 11/3/2016 5:22 PM
ms.date: 11/3/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/MSOnline/v1/Get-MsolDomainVerificationDns.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/cedef1609da4230592c00be27ccc62e342e2df61/Azure%20AD%20Cmdlets/MSOnline/v1/Get-MsolDomainVerificationDns.md
ms.topic: reference
ms.prod: powershell
ms.service: Azure PowerShell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-MsolDomainVerificationDns

## SYNOPSIS
Retrieves a list of records to configure a domain.

## SYNTAX

```
Get-MsolDomainVerificationDns -DomainName <String> [-Mode <DomainVerificationMode>] [-TenantId <Guid>]
 [<CommonParameters>]
```

## DESCRIPTION
The Get-MsolDomainVerificationDns cmdlet is used to return the DNS records that need to be set to verify a domain.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Get-MsolDomainVerificationDNS -DomainName contoso.com

          Returns the DNS record.
```

Description

-----------

This command retrieves the DNS records that need to be set in order to verify ownership of contoso.com.

## PARAMETERS

### -DomainName
The fully qualified domain name to retrieve.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Mode
The domain verification mode to use when verifying this domain.
Possible values for Mode are DnsMXRecord and DnsTxtRecord.

```yaml
Type: DomainVerificationMode
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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.Online.Administration.DomainRecord
This cmdlet returns details about the DNS records required to verify a domain.

## NOTES

## RELATED LINKS


