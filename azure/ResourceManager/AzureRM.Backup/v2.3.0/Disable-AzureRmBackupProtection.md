---
external help file: Microsoft.Azure.Commands.AzureBackup.dll-Help.xml
ms.assetid: F8849412-61CD-42E0-9A00-48F5D885B826
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Backup/v2.3.0/Disable-AzureRmBackupProtection.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.Backup/v2.3.0/Disable-AzureRmBackupProtection.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: ResourceManager_AzureRM_Backup_v2_3_0_Disable_AzureRmBackupProtection_md
---

# Disable-AzureRmBackupProtection

## SYNOPSIS
Disables protection for a Backup protected item.

## SYNTAX

```
Disable-AzureRmBackupProtection [-RemoveRecoveryPoints] [-Force] [-Item] <AzureRMBackupItem> [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Disable-AzureRmBackupProtection** cmdlet disables protection for an Azure Backup protected item.
This cmdlet stops regular scheduled backup of an item.
This cmdlet can delete existing recovery points for the backup item.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -Force
Forces the command to run without asking for user confirmation.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Item
Specifies the Backup item for which this cmdlet disables protection.
To obtain an **AzureRmBackupItem**, use the Get-AzureRmBackupItem cmdlet.

```yaml
Type: AzureRMBackupItem
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -RemoveRecoveryPoints
Indicates that this cmdlet deletes existing recovery points.
To delete stored recovery points later, run this cmdlet again and specify this parameter.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### AzureRmBackupItem

## OUTPUTS

### AzureRmBackupJob

## NOTES

## RELATED LINKS

[Enable-AzureRmBackupProtection](xref:ResourceManager/AzureRM.Backup/v2.3.0/Enable-AzureRmBackupProtection.md)

[Get-AzureRmBackupItem](xref:ResourceManager/AzureRM.Backup/v2.3.0/Get-AzureRmBackupItem.md)


