---
external help file: Microsoft.Azure.Commands.HDInsight.dll-Help.xml
ms.assetid: 692AD3AD-8C5A-4747-869D-2BDDDCC3AAAD
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.HDInsight/v2.3.0/Get-AzureRmHDInsightPersistedScriptAction.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.HDInsight/v2.3.0/Get-AzureRmHDInsightPersistedScriptAction.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: ResourceManager_AzureRM_HDInsight_v2_3_0_Get_AzureRmHDInsightPersistedScriptAction_md
---

# Get-AzureRmHDInsightPersistedScriptAction

## SYNOPSIS
Gets the persisted script actions for a cluster and lists them in chronological order, or gets details for a specified persisted script action.

## SYNTAX

```
Get-AzureRmHDInsightPersistedScriptAction [-ClusterName] <String> [[-Name] <String>]
 [-ResourceGroupName <String>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmHDInsightPersistedScriptAction** cmdlet gets the persisted script actions for an Azure HDInsight cluster and lists them in chronological order, or gets details for a specified persisted script action.

## EXAMPLES

### Example 1: Get the persisted script actions on a cluster
```
PS C:\>Get-AzureRmHDInsightPersistedScriptAction -ClusterName "your-hadoop-001"
```

This command gets persisted script actions on the cluster named your-hadoop-001.

## PARAMETERS

### -ClusterName
Specifies the name of the cluster.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the name of the persisted script action.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group.

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

### -InformationAction
Specifies how this cmdlet responds to an information event.

The acceptable values for this parameter are:

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

[Remove-AzureRmHDInsightPersistedScriptAction](xref:ResourceManager/AzureRM.HDInsight/v2.3.0/Remove-AzureRmHDInsightPersistedScriptAction.md)

[Set-AzureRmHDInsightPersistedScriptAction](xref:ResourceManager/AzureRM.HDInsight/v2.3.0/Set-AzureRmHDInsightPersistedScriptAction.md)


