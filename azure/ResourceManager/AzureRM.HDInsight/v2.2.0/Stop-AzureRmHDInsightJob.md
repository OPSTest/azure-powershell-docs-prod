---
external help file: Microsoft.Azure.Commands.HDInsight.dll-Help.xml
online version: 3bc9e3a9-d8e6-4cad-8642-4bea508a6ba1
schema: 2.0.0
ms.assetid: DC11783A-8DB6-488B-A493-132F7E91FF5D
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.HDInsight/v2.2.0/Stop-AzureRmHDInsightJob.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.HDInsight/v2.2.0/Stop-AzureRmHDInsightJob.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: 
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Stop-AzureRmHDInsightJob

## SYNOPSIS
Stops a specified running job on a cluster.

## SYNTAX

```
Stop-AzureRmHDInsightJob [-ClusterName] <String> [-JobId] <String> [-HttpCredential] <PSCredential>
 [-ResourceGroupName <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Stop-AzureRmHDInsightJob** cmdlet stops a specified running job on an Azure HDInsight cluster.

## EXAMPLES

### Example 1: Stop a job on the specified cluster
```
PS C:\># Cluster info
PS C:\> $clusterName = "your-hadoop-001"
PS C:\> $clusterCreds = Get-Credential
PS C:\> Stop-AzureRmHDInsightJob `
            -ClusterName $clusterName `
            -ClusterCredential $clusterCreds `
            -JobId $jobId
```

This command stops a job on the cluster named your-hadoop-001.

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

### -JobId
Specifies the job ID of the job.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -HttpCredential
Specifies the cluster login (HTTP) credentials for the cluster.

```yaml
Type: PSCredential
Parameter Sets: (All)
Aliases: ClusterCredential

Required: True
Position: 2
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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmHDInsightJob](xref:ResourceManager/AzureRM.HDInsight/v2.2.0/Get-AzureRmHDInsightJob.md)

[Start-AzureRmHDInsightJob](xref:ResourceManager/AzureRM.HDInsight/v2.2.0/Start-AzureRmHDInsightJob.md)

[Wait-AzureRmHDInsightJob](xref:ResourceManager/AzureRM.HDInsight/v2.2.0/Wait-AzureRmHDInsightJob.md)


