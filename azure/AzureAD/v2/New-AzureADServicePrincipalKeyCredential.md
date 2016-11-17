---
external help file: Microsoft.Open.AzureAD16.Graph.PowerShell.Custom.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: D6EA0D4D-6643-4F11-A94C-2A71827C2774
updated_at: 11/8/2016 7:03 PM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/live/Azure%20AD%20Cmdlets/AzureAD/v2/New-AzureADServicePrincipalKeyCredential.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/a065a4a5ac7da74bf8a17be84ad0723ab28e24cb/Azure%20AD%20Cmdlets/AzureAD/v2/New-AzureADServicePrincipalKeyCredential.md
ms.topic: reference
ms.prod: 
ms.service: active-directory
ms.technology: Azure PowerShell
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: carolz
id: AzureAD_v2_New_AzureADServicePrincipalKeyCredential_md
---

# New-AzureADServicePrincipalKeyCredential

## SYNOPSIS
Create a new key credential for a service principal

## SYNTAX

```
New-AzureADServicePrincipalKeyCredential -ObjectId <String> [-CustomKeyIdentifier <String>]
 [-StartDate <DateTime>] [-EndDate <DateTime>] [-Type <KeyType>] [-Usage <KeyUsage>] [-Value <String>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureADServicePrincipalKeyCredential** cmdlet creates a key credential for a service principal in Azure Active Directory (AD).
## EXAMPLES

### Example 1: Create a key credential
```PowerShell
PS C:\>New-AzureADServicePrincipalKeyCredential
```
This command creates a key credential for a service principal.
## PARAMETERS

### -ObjectId
Specifies an object ID.

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

### -CustomKeyIdentifier


```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -StartDate


```yaml
Type: DateTime
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -EndDate


```yaml
Type: DateTime
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Type


```yaml
Type: KeyType
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Usage

```yaml
Type: KeyUsage
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Value

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
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
[Get-AzureADServicePrincipalKeyCredential](xref:AzureAD/v2/Get-AzureADServicePrincipalKeyCredential.md)

[Remove-AzureADServicePrincipalKeyCredential](xref:AzureAD/v2/Remove-AzureADServicePrincipalKeyCredential.md)
