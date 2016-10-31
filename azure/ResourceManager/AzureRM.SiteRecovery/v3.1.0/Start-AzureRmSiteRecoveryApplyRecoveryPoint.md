---
external help file: Microsoft.Azure.Commands.SiteRecovery.dll-Help.xml
online version: 2cd9e814-4020-4ca5-ab45-855f15c1d3eb
schema: 2.0.0
ms.assetid: 938501F5-0726-4DEB-889B-2068FF5ED198
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.SiteRecovery/v3.1.0/Start-AzureRmSiteRecoveryApplyRecoveryPoint.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.SiteRecovery/v3.1.0/Start-AzureRmSiteRecoveryApplyRecoveryPoint.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Start-AzureRmSiteRecoveryApplyRecoveryPoint

## SYNOPSIS
Changes a recovery point for a failed over protected item before commiting the failover operation.

## SYNTAX

```
Start-AzureRmSiteRecoveryApplyRecoveryPoint -RecoveryPoint <ASRRecoveryPoint>
 -ReplicationProtectedItem <ASRReplicationProtectedItem> [-DataEncryptionPrimaryCertFile <String>]
 [-DataEncryptionSecondaryCertFile <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Start-AzureRmSiteRecoveryApplyRecoveryPoint** changes a recovery point for a failed over protected item before it commits the failover operation.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -RecoveryPoint
Specifies the recovery point object that this cmdlet changes.

```yaml
Type: ASRRecoveryPoint
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ReplicationProtectedItem
Specifies the Replication Protected Item object.

```yaml
Type: ASRReplicationProtectedItem
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -DataEncryptionPrimaryCertFile
@{Text=}

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DataEncryptionSecondaryCertFile
@{Text=}

```yaml
Type: String
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

### Microsoft.Azure.Commands.SiteRecovery.ASRJob

## NOTES

## RELATED LINKS

[Azure Site Recovery Cmdlets](xref:ResourceManager/AzureRM.SiteRecovery/v3.1.0/AzureRM.SiteRecovery.md)


