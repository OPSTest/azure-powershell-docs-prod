---
external help file: Microsoft.Azure.Commands.Scheduler.dll-Help.xml
online version: 0324dd5f-1c8d-4f82-9ffa-292e304578ff
schema: 2.0.0
ms.assetid: 12988A40-422A-4E32-9798-DEEEB2C21009
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Scheduler/v0.11.0/Get-AzureRmSchedulerJobHistory.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Scheduler/v0.11.0/Get-AzureRmSchedulerJobHistory.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureRmSchedulerJobHistory

## SYNOPSIS
Gets job history.

## SYNTAX

```
Get-AzureRmSchedulerJobHistory -ResourceGroupName <String> -JobCollectionName <String> -JobName <String>
 [-JobExecutionStatus <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmSchedulerJobHistory** cmdlet gets history for an Azure Scheduler job.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -ResourceGroupName
Specifies the resource group to which the job belongs.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -JobCollectionName
Specifies the name of a job collection.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Name, ResourceName

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -JobName
Specifies the name of a job for which this cmdlet gets history.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -JobExecutionStatus
Specifies the status of a job.
This cmdlet gets history that matches the status that you specify.
The acceptable values for this parameter are:

- Completed 
- Failed 
- Postponed

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmSchedulerJob](xref:ResourceManager/AzureRM.Scheduler/v0.11.0/Get-AzureRmSchedulerJob.md)


