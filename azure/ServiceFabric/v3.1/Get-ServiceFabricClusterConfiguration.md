---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
online version: .\Connect-ServiceFabricCluster.md
schema: 2.0.0
ms.assetid: 13C206CD-D1A4-4BAE-8014-4D7AB68D147D
updated_at: 10/18/2016 11:23 PM
ms.date: 10/18/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/v3.1/Get-ServiceFabricClusterConfiguration.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/a1c583c96910e336e02325104794c31c6626c552/Service-Fabric-cmdlets/ServiceFabric/v3.1/Get-ServiceFabricClusterConfiguration.md
ms.topic: reference
ms.prod: powershell
ms.service: service-fabric
ms.technology: Azure Powershell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-ServiceFabricClusterConfiguration

## SYNOPSIS
Retrieves the latest JSON cluster configuration.

## SYNTAX

```
Get-ServiceFabricClusterConfiguration [-TimeoutSec <Int32>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-ServiceFabricClusterConfiguration** cmdlet retrieves the latest cluster configuration in JavaScript Object Notation (JSON) format.
To run this cmdlet, you must first establish a connection by using the Connect-ServiceFabricCluster cmdlet.

## EXAMPLES

### Example 1: Get cluster configuration
```
PS C:\>Connect-ServiceFabricCluster -ConnectionEndpoint "ServiceFabric01.ContosoCloudApp.net:19000"
PS C:\> Get-ServiceFabricClusterConfiguration
```

The first command creates a connection to the specified cluster.

The second command gets the latest cluster configuration in JSON format.

## PARAMETERS

### -TimeoutSec
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

[Connect-ServiceFabricCluster](.\Connect-ServiceFabricCluster.md)

[Get-ServiceFabricClusterConfigurationUpgradeStatus](.\Get-ServiceFabricClusterConfigurationUpgradeStatus.md)

[Start-ServiceFabricClusterConfigurationUpgrade](.\Start-ServiceFabricClusterConfigurationUpgrade.md)

