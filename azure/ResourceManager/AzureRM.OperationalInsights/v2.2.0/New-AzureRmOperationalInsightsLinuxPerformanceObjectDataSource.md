---
external help file: Microsoft.Azure.Commands.OperationalInsights.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: F54F6B48-64B5-4EAF-BAFE-819B4CBF42B9
updated_at: 11/1/2016 10:24 PM
ms.date: 11/1/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.OperationalInsights/v2.2.0/New-AzureRmOperationalInsightsLinuxPerformanceObjectDataSource.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/f59f3ef60bc592383812213e69fd77ba950759ed/azureps-cmdlets-docs/ResourceManager/AzureRM.OperationalInsights/v2.2.0/New-AzureRmOperationalInsightsLinuxPerformanceObjectDataSource.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: ResourceManager_AzureRM_OperationalInsights_v2_2_0_New_AzureRmOperationalInsightsLinuxPerformanceObjectDataSource_md
---

# New-AzureRmOperationalInsightsLinuxPerformanceObjectDataSource

## SYNOPSIS
Adds performance counters to all Linux computers in a workspace.

## SYNTAX

### ByWorkspaceName (Default)
```
New-AzureRmOperationalInsightsLinuxPerformanceObjectDataSource [-ObjectName] <String>
 [[-InstanceName] <String>] [-CounterNames] <String[]> [[-IntervalSeconds] <Int32>] [-Name] <String>
 [-ResourceGroupName] <String> [-WorkspaceName] <String> [-Force] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### ByWorkspaceObject
```
New-AzureRmOperationalInsightsLinuxPerformanceObjectDataSource [-ObjectName] <String>
 [[-InstanceName] <String>] [-CounterNames] <String[]> [[-IntervalSeconds] <Int32>] [-Name] <String>
 [-Workspace] <PSWorkspace> [-Force] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureRmOperationalInsightsLinuxPerformanceObjectDataSource** cmdlet adds performance counters from which Azure Operational Insights collects data to all Linux computers in a workspace.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -ObjectName
Specifies the name of an object.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 4
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -InstanceName
Specifies an instance name.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 5
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -CounterNames
Specifies an array of names of counters.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: True
Position: 6
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -IntervalSeconds
Specifies the interval of collection.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: 7
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies a name for the data source.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of a resource group that contains Linux computers.

```yaml
Type: String
Parameter Sets: ByWorkspaceName
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -WorkspaceName
Specifies the name of a workspace in which this cmdlet operates.

```yaml
Type: String
Parameter Sets: ByWorkspaceName
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

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

### -Workspace
Specifies a workspace in which this cmdlet operates.

```yaml
Type: PSWorkspace
Parameter Sets: ByWorkspaceObject
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Disable-AzureRmOperationalInsightsLinuxPerformanceCollection](xref:ResourceManager/AzureRM.OperationalInsights/v2.2.0/Disable-AzureRmOperationalInsightsLinuxPerformanceCollection.md)

[Enable-AzureRmOperationalInsightsLinuxPerformanceCollection](xref:ResourceManager/AzureRM.OperationalInsights/v2.2.0/Enable-AzureRmOperationalInsightsLinuxPerformanceCollection.md)


