---
external help file: Microsoft.Online.Identity.Federation.PowerShell.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 623D0291-0C85-422F-BC47-43D019839C16
updated_at: 11/3/2016 5:22 PM
ms.date: 11/3/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/MSOnline/v1/New-MsolFederatedDomain.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/cedef1609da4230592c00be27ccc62e342e2df61/Azure%20AD%20Cmdlets/MSOnline/v1/New-MsolFederatedDomain.md
ms.topic: reference
ms.prod: powershell
ms.service: Azure PowerShell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# New-MsolFederatedDomain

## SYNOPSIS
Adds a new single sign-on domain (also known as identity-federated domain) to Microsoft Online Services and establishes the relying party trust between the Active Directory Federation Services 2.0 server and Microsoft Online.

## SYNTAX

```
New-MsolFederatedDomain [-SupportMultipleDomain] -DomainName <String> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The Add-MSOLFederatedDomain cmdlet adds a new single sign-on domain (also known as identity-federated domain) to Microsoft Online Services and configures the relying party trust settings between the on-premises Active Directory Federation Services 2.0 server and Microsoft Online.
Due to domain verification requirements, you may need to run this cmdlet several times in order to complete the process of adding the new single sign-on domain.

## PARAMETERS

### -DomainName
The name of the new single sign-on domain (also known as identity-federated domain) to create in Microsoft Online.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SupportMultipleDomain


```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before executing the command.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Describes what would happen if you executed the command without actually executing the command.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

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


