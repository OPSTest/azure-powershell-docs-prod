---
external help file: Microsoft.Open.AzureAD16.Graph.PowerShell.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: D4C305FF-6005-4296-8B26-CFFCACFF9D2C
updated_at: 11/7/2016 8:58 PM
ms.date: 11/7/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/live/Azure%20AD%20Cmdlets/AzureAD/v2/Get-AzureADServicePrincipalPolicy.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/414ab491f42a4ba60faf9f10b89c4e7ebf47654a/Azure%20AD%20Cmdlets/AzureAD/v2/Get-AzureADServicePrincipalPolicy.md
ms.topic: reference
ms.prod: 
ms.service: active-directory
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureADServicePrincipalPolicy

## SYNOPSIS

## SYNTAX

```
Get-AzureADServicePrincipalPolicy -ObjectId <String> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureADServicePrincipalPolicy** cmdlet gets the policy of a service principal in Azure Active Directory (AD).
## EXAMPLES

### Example 1: Get a policy
```PowerShell
PS C:\>Get-AzureADServicePrincipalPolicy -ObjectId "<object id of service principal>"
```
This command get the policy for the specified service principal.
## PARAMETERS

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
[Add-AzureADServicePrincipalPolicy](xref:AzureAD/v2/Add-AzureADServicePrincipalPolicy.md)

[Remove-AzureADServicePrincipalPolicy](xref:AzureAD/v2/Remove-AzureADServicePrincipalPolicy.md)

