---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
online version: ./Connect-ServiceFabricCluster.md
schema: 2.0.0
ms.assetid: FD4821A9-3C2A-4AFB-9611-D46FF1D4772C
updated_at: 10/24/2016 10:54 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Test-ServiceFabricClusterManifest.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/865a3e19e58e9be5871c4d9834591e4ba1c1b9ec/Service-Fabric-cmdlets/ServiceFabric/vlatest/Test-ServiceFabricClusterManifest.md
ms.topic: reference
ms.prod: powershell
ms.service: service-fabric
ms.technology: Azure Powershell
author: visual-studio-china
ms.author: 
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Test-ServiceFabricClusterManifest

## SYNOPSIS
Validates a Service Fabric cluster manifest.

## SYNTAX

```
Test-ServiceFabricClusterManifest [-ClusterManifestPath] <String> [-OldClusterManifestPath <String>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Test-ServiceFabricClusterManifest** cmdlet validates a Service Fabric cluster manifest.
In order to help avoid issues with a Service Fabric upgrade, we recommended that you test a new cluster manifest for obvious errors.
This cmdlet does not discover issues with configuration values.

## EXAMPLES

### Example 1: Validate a cluster manifest
```
PS C:\>Test-ServiceFabricClusterManifest -ClusterManifestPath \\configStore\ClusterManifests\CH1\ClusterManifest_123.xml
```

This command validates a Service Fabric cluster manifest.
The command specifies a manifest location on a network share.

### Example 2: Validate an updated cluster manifest
```
PS C:\>Test-ServiceFabricClusterManifest -ClusterManifestPath \\configStore\ClusterManifests\CH1\ClusterManifest_123.v2.xml -OldClusterManifestPath \\configStore\ClusterManifests\CH1\ClusterManifest_123.v1.xml
```

This command validates a Service Fabric cluster manifest upgrade.
The command specifies a new cluster manifest location and an old cluster manifest location on a network share.

## PARAMETERS

### -ClusterManifestPath
Specifies the path of a Service Fabric cluster manifest.
The cmdlet validates the manifest in the path that you specify.

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

### -OldClusterManifestPath
Specifies the path of a Service Fabric cluster manifest that is already deployed.
The cmdlet validates the manifest that is specified by the *ClusterManifestPath* parameter against the manifest that this parameter specifies for configuration upgrade purposes.

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

### None
You cannot pipe input to this cmdlet.

## OUTPUTS

### System.Object
This cmdlet returns $True if the Service Fabric cluster manifest is valid, or, if it is not valid, this cmdlet returns $False.

## NOTES

## RELATED LINKS

[Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md)

[Get-ServiceFabricClusterConnection](./Get-ServiceFabricClusterConnection.md)

[Get-ServiceFabricClusterManifest](./Get-ServiceFabricClusterManifest.md)


