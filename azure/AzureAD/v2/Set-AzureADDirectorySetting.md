---
external help file: Microsoft.Open.MS.GraphBeta.PowerShell.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 96F47B05-3D04-4298-9C60-03B60B8AD6AF
updated_at: 11/10/2016 7:13 PM
ms.date: 11/10/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2/Set-AzureADDirectorySetting.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/0fe9adfb52ba045c8e77b8982014c103a8c0c6f3/Azure%20AD%20Cmdlets/AzureAD/v2/Set-AzureADDirectorySetting.md
ms.topic: reference
ms.prod: 
ms.service: active-directory
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: AzureAD_v2_Set_AzureADDirectorySetting_md
---

# Set-AzureADDirectorySetting

## SYNOPSIS
Updates a directory setting in Azure Active Directory.

## SYNTAX

```
Set-AzureADDirectorySetting [-ObjectId <String>] -DirectorySetting <DirectorySetting>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureADDirectorySetting** cmdlet updates a directory setting in Azure Active Directory (AD).


## PARAMETERS

### -ObjectId
Specifies the ID of a settings object in Azure AD.

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

### -DirectorySetting
Specifies the directory settings.

```yaml
Type: DirectorySetting
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
[Get-AzureADDirectorySetting](xref:AzureAD/v2/Get-AzureADDirectorySetting.md)

[New-AzureADDirectorySetting](xref:AzureAD/v2/New-AzureADDirectorySetting.md)

[Remove-AzureADDirectorySetting](xref:AzureAD/v2/Remove-AzureADDirectorySetting.md)
