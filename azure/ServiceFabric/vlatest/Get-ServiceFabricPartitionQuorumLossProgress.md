---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
online version: ./Start-ServiceFabricPartitionQuorumLoss.md
schema: 2.0.0
ms.assetid: A3614BE3-5C8A-419D-BAD4-01B1443248A9
updated_at: 10/24/2016 10:54 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricPartitionQuorumLossProgress.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/865a3e19e58e9be5871c4d9834591e4ba1c1b9ec/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricPartitionQuorumLossProgress.md
ms.topic: reference
ms.prod: powershell
ms.service: service-fabric
ms.technology: Azure Powershell
author: visual-studio-china
ms.author: 
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-ServiceFabricPartitionQuorumLossProgress

## SYNOPSIS
Gets the progress of a quorum loss operation.

## SYNTAX

```
Get-ServiceFabricPartitionQuorumLossProgress -OperationId <Guid> [-TimeoutSec <Int32>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-ServiceFabricPartitionQuorumLossProgress** cmdlet gets the progress of a quorum loss operation in Azure Service Fabric.
Initiate a quorum loss operation by using the Start-ServiceFabricPartitionQuorumLoss cmdlet.

## EXAMPLES

### Example 1: Check progress of quorum loss operation
```
PS C:\>Get-ServiceFabricPartitionQuorumLossProgress -OperationId aeaceca9-320d-4f7b-84e8-3cc13c29a974
  State Result
  ----- ------
Running
```

This command checks the progress of a quorum loss operation that has the ID aeaceca9-320d-4f7b-84e8-3cc13c29a974.
The operation is still running.

## PARAMETERS

### -OperationId
Specifies a unique identifier for the operation that this cmdlet checks.
You assign this value when you run **Start-ServiceFabricPartitionQuorumLoss**.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TimeoutSec
Specifies the time-out period, in seconds, for the operation.

```yaml
Type: Int32
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

[Start-ServiceFabricPartitionQuorumLoss](./Start-ServiceFabricPartitionQuorumLoss.md)


