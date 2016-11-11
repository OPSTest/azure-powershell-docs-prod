---
external help file: Microsoft.Azure.Commands.Cdn.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: A05FA90C-3B36-4359-8C31-5DF293B4CAE1
updated_at: 11/1/2016 10:24 PM
ms.date: 11/1/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Cdn/v2.2.0/Get-AzureRmCdnProfileSsoUrl.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/f59f3ef60bc592383812213e69fd77ba950759ed/azureps-cmdlets-docs/ResourceManager/AzureRM.Cdn/v2.2.0/Get-AzureRmCdnProfileSsoUrl.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: ResourceManager_AzureRM_Cdn_v2_2_0_Get_AzureRmCdnProfileSsoUrl_md
---

# Get-AzureRmCdnProfileSsoUrl

## SYNOPSIS
Gets the single sign-on URL of a CDN profile.

## SYNTAX

### Parameter Set for fields parameters (Default)
```
Get-AzureRmCdnProfileSsoUrl -ProfileName <String> -ResourceGroupName <String> [<CommonParameters>]
```

### Parameter Set for object parameters
```
Get-AzureRmCdnProfileSsoUrl -CdnProfile <PSProfile> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmCdnProfileSsoUrl** cmdlet gets the single sign-on URL of the Azure Content Delivery Network (CDN) profile.
This URL lets users conntect to a supplementary portal and use additional features of  CDN.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -ProfileName
Specifies the name of the CDN profile.

```yaml
Type: String
Parameter Sets: Parameter Set for fields parameters
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group name to which the profile belongs.

```yaml
Type: String
Parameter Sets: Parameter Set for fields parameters
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CdnProfile
Specifies the CDN profile.

```yaml
Type: PSProfile
Parameter Sets: Parameter Set for object parameters
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

###  
This cmdlet returns a URL.

## NOTES

## RELATED LINKS

[Get-AzureRMCdnProfile](xref:ResourceManager/AzureRM.Cdn/v2.2.0/Get-AzureRMCdnProfile.md)


