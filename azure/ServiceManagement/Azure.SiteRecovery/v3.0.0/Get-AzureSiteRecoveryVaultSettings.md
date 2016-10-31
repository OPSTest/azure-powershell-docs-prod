---
external help file: Microsoft.Azure.Commands.RecoveryServicesRdfe.dll-Help.xml
online version: bc42aab9-738f-4eb9-90f3-9ad054075927
schema: 2.0.0
ms.assetid: 0267B77A-F6EE-43B8-9B22-3D71AC453A66
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.SiteRecovery/v3.0.0/Get-AzureSiteRecoveryVaultSettings.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.SiteRecovery/v3.0.0/Get-AzureSiteRecoveryVaultSettings.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureSiteRecoveryVaultSettings

## SYNOPSIS
Gets settings information about an Azure Site Recovery vault.

## SYNTAX

```
Get-AzureSiteRecoveryVaultSettings [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureSiteRecoveryVaultSettings** cmdlet gets settings information about a Microsoft Azure Site Recovery vault.

## EXAMPLES

### Example 1: Get settings information
```
PS C:\>Get-AzureSiteRecoveryVaultSettings
ResourceName                                                CloudServiceName
------------                                                ----------------
ContosoVault                                                RecoveryServices-6JP23WE3SKKOM5AFQG2YQAI22MNOWK52QDKWMUP...
```

This command gets settings information for the current Azure Site Recovery vault.

## PARAMETERS

### -Profile
Specifies an Azure profile.

```yaml
Type: AzureSMProfile
Parameter Sets: (All)
Aliases: 

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

[Import-AzureSiteRecoveryVaultSettingsFile](xref:ServiceManagement/Azure.SiteRecovery/v3.0.0/Import-AzureSiteRecoveryVaultSettingsFile.md)


