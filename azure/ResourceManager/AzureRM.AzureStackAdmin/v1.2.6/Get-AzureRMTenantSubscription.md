---
external help file: Microsoft.AzureStack.Commands.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 346CA4A0-3ABF-4257-8F04-E7651ACD0A06
updated_at: 11/11/2016 11:03 PM
ms.date: 11/11/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.AzureStackAdmin/v1.2.6/Get-AzureRMTenantSubscription.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/79eeb985ea480979357fb4695832a0c3d29a48bf/azureps-cmdlets-docs/ResourceManager/AzureRM.AzureStackAdmin/v1.2.6/Get-AzureRMTenantSubscription.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: ResourceManager_AzureRM_AzureStackAdmin_v1_2_6_Get_AzureRMTenantSubscription_md
---

# Get-AzureRMTenantSubscription

## SYNOPSIS
The Get-AzureRmTenantSubscription gets the subscriptions associated with the current logged in user.

## SYNTAX

```
Get-AzureRMTenantSubscription [-AdminUri <Uri>] [-Token <String>] [-ApiVersion <String>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [-PipelineVariable <String>]
```

## DESCRIPTION

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Get-AzureRmTenantSubscription
```

Description

-----------

Simply execute Get-AzureRmTenantSubscription after logging in with Add-AzureRmAccount

## PARAMETERS

### -AdminUri
Specifies the azure stack resource manager endpoint.
This parameter is not needed when using the cmdlet against the azure stack environment configured against azure active directory

```yaml
Type: Uri
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ApiVersion
Specifies the api version supported.
This is optional.
This parameter will be deprecated in future

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -InformationAction
Not Specified

The following values are permitted for this object type.

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa
Accepted values: SilentlyContinue, Stop, Continue, Inquire

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
Not Specified

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

### -PipelineVariable
Not Specified

```yaml
Type: String
Parameter Sets: (All)
Aliases: pv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Token
Authentication token for making the request.
This parameter is not needed when using the cmdlet against the azure stack environment configured against azure active directory. 
This parameter will be deprecated in a future release

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

### Microsoft.AzureStack.Management.Models.SubscriptionDefinition

## NOTES
## RELATED LINKS

