---
external help file: Microsoft.Open.AzureAD16.Graph.PowerShell.Custom.dll-Help.xml
ms.assetid: AB894D03-378C-4F96-87C2-54FA2C7476B3
online version: 
schema: 2.0.0
updated_at: 11/19/2016 5:55 PM
ms.date: 11/19/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2/Remove-AzureADServicePrincipalKeyCredential.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/78576a00e7eab32d13180fb832c5e222accdc9ce/Azure%20AD%20Cmdlets/AzureAD/v2/Remove-AzureADServicePrincipalKeyCredential.md
ms.topic: reference
ms.prod: 
ms.service: active-directory
ms.technology: Azure PowerShell
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: carolz
id: AzureAD_v2_Remove_AzureADServicePrincipalKeyCredential_md
---

# Remove-AzureADServicePrincipalKeyCredential

## SYNOPSIS
Removes a key credential from a service principal.

## SYNTAX

```
Remove-AzureADServicePrincipalKeyCredential -ObjectId <String> -KeyId <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureADServicePrincipalKeyCredential** cmdlet removes a key credential from a service principal in Azure Active Directory (AD).

## EXAMPLES

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

### -KeyId
Specifies the ID of a key credential.

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

### -ObjectId
Specifies the ID of a service principal.

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

[Get-AzureADServicePrincipalKeyCredential](xref:AzureAD/v2/Get-AzureADServicePrincipalKeyCredential.md)

[New-AzureADServicePrincipalKeyCredential](xref:AzureAD/v2/New-AzureADServicePrincipalKeyCredential.md)
