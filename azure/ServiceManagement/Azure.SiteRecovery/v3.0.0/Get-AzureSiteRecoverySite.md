---
external help file: Microsoft.Azure.Commands.RecoveryServicesRdfe.dll-Help.xml
online version: 8714ec35-9048-475c-83f5-0c2a1790740b
schema: 2.0.0
ms.assetid: 1135F4D4-C7A4-4ECB-BF4D-EECC8C32EDE4
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.SiteRecovery/v3.0.0/Get-AzureSiteRecoverySite.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.SiteRecovery/v3.0.0/Get-AzureSiteRecoverySite.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureSiteRecoverySite

## SYNOPSIS
Gets Azure Site Recovery sites in a vault.

## SYNTAX

```
Get-AzureSiteRecoverySite [-Vault <ASRVault>] [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureSiteRecoverySite** cmdlet gets Azure Site Recovery sites in an Azure Site Recovery vault.

## EXAMPLES

### Example 1: Get recovery sites
```
PS C:\>Get-AzureSiteRecoverySite
Type                                    Name                                    ID
----                                    ----                                    --
HyperVSite                              RecoverySite07                          f16829b4-5b01-4209-a6cf-8e0aff1fe328
```

This command gets the recovery sites for the current vault.

## PARAMETERS

### -Vault
Specifies a vault for which to get sites.
To obtain an **ASRVault** object, use the **Get-AzureSiteRecoveryVault** cmdlet.

```yaml
Type: ASRVault
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

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

[New-AzureSiteRecoverySite](./New-AzureSiteRecoverySite.md)

[Get-AzureSiteRecoveryVault](./Get-AzureSiteRecoveryVault.md)


