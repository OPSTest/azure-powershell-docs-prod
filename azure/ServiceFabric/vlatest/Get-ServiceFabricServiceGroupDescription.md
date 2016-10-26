---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
online version: ./New-ServiceFabricServiceGroup.md
schema: 2.0.0
ms.assetid: 9226A922-F033-4916-9588-D6BE73ED6F67
updated_at: 10/24/2016 10:54 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricServiceGroupDescription.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/865a3e19e58e9be5871c4d9834591e4ba1c1b9ec/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricServiceGroupDescription.md
ms.topic: reference
ms.prod: powershell
ms.service: service-fabric
ms.technology: Azure Powershell
author: visual-studio-china
ms.author: 
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-ServiceFabricServiceGroupDescription

## SYNOPSIS
Gets a Service Fabric service group description.

## SYNTAX

```
Get-ServiceFabricServiceGroupDescription [-ServiceName] <Uri> [-TimeoutSec <Int32>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-ServiceFabricServiceGroupDescription** cmdlet gets the Service Fabric service group description of a service that is running.

Before you perform any operation on a Service Fabric cluster, establish a connection to the cluster by using the Connect-ServiceFabricCluster cmdlet.

## EXAMPLES

### Example 1: Get a service group description
```
PS C:\>Get-ServiceFabricServiceGroupDescription -ServiceName fabric:/CalcApp/CalcService
```

This command gets the Service Fabric service group description for the service named fabric:/CalcApp/CalcService.

## PARAMETERS

### -ServiceName
Specifies the Uniform Resource Identifier (URI) of a Service Fabric service group.

```yaml
Type: Uri
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
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

### System.Uri
This cmdlet accepts a URI that represents the name of a Service Fabric service group.

## OUTPUTS

### System.Object
This cmdlet returns a **System.Fabric.Description.ServiceGroupDescription** object for a Service Fabric service group.

## NOTES

## RELATED LINKS

[New-ServiceFabricServiceGroup](./New-ServiceFabricServiceGroup.md)

[Remove-ServiceFabricServiceGroup](./Remove-ServiceFabricServiceGroup.md)

[Update-ServiceFabricServiceGroup](./Update-ServiceFabricServiceGroup.md)


