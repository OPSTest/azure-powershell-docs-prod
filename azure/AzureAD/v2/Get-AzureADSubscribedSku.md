---
external help file: Microsoft.Open.AzureAD16.Graph.PowerShell.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 0E1A27BF-2CD9-43CD-851D-D1F09484CDE3
updated_at: 11/7/2016 9:42 PM
ms.date: 11/7/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2/Get-AzureADSubscribedSku.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/3fe29818e79701638ab0561b0255471c0715c67b/Azure%20AD%20Cmdlets/AzureAD/v2/Get-AzureADSubscribedSku.md
ms.topic: reference
ms.prod: 
ms.service: active-directory
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: AzureAD_v2_Get_AzureADSubscribedSku_md
---

# Get-AzureADSubscribedSku

## SYNOPSIS
Gets subscribed SKUs to Microsoft services.

## SYNTAX

```
Get-AzureADSubscribedSku [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureADSubscribedSku** cmdlet gets subscribed SKUs to Microsoft services.
## EXAMPLES

### Example 1: Get subscribed SKUs
```PowerShell
PS C:\>Get-AzureADSubscribedSku

ObjectId                                                                  SkuPartNumber         PrepaidUnits                                                             ConsumedUnits
--------                                                                  -------------         ------------                                                             -------------
85b5ff1e-0402-400c-9e3c-0f9e965325d1_078d2b04-f1bd-4111-bbd4-b4b1b354cef4 AAD_PREMIUM           class LicenseUnitsDetail {... 
6
85b5ff1e-0402-400c-9e3c-0f9e965325d1_f245ecc8-75af-4f8e-b61f-27d8114de5f3 O365_BUSINESS_PREMIUM class LicenseUnitsDetail {... 
24
```
This command gets subscribed SKUs.
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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS


