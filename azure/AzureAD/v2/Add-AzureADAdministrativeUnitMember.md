---
external help file: Microsoft.Open.AzureADBeta.Graph.PowerShell.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: C2254A89-1700-4321-99FD-529E481705A3
updated_at: 11/1/2016 10:50 PM
ms.date: 11/1/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2/Add-AzureADAdministrativeUnitMember.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/dddb54a925d64a5a3ede382c93d53550f9d8428e/Azure%20AD%20Cmdlets/AzureAD/v2/Add-AzureADAdministrativeUnitMember.md
ms.topic: reference
ms.prod: powershell
ms.service: Azure PowerShell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Add-AzureADAdministrativeUnitMember

## SYNOPSIS
Adds an administrative unit member.

## SYNTAX

```
Add-AzureADAdministrativeUnitMember -ObjectId <String> -RefObjectId <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Add-AzureADAdministrativeUnitMember** cmdlet adds an Active Directory administrative unit member.

## PARAMETERS

### -ObjectId
Specifies the ID of an Active Directory administrative unit.
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

### -RefObjectId
Specifies the unique ID of the specific Azure Active Directory object that will be assigned as owner/manager/member.
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
Specifies how this cmdlet responds to an information event.
The acceptable values for this parameter are:
* Continue
* Ignore
* Inquire
* SilentlyContinue
* Stop
* Suspend
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
Specifies a variable in which to store an information event message.
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
<a href="https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2/Get-AzureADAdministrativeUnitMember.md" title="example">Get-AzureADAdministrativeUnitMember</a><br>
<a href="https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2/Remove-AzureADAdministrativeUnitMember.md" title="example">Remove-AzureADAdministrativeUnitMember</a><br>
