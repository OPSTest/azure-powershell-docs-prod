---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
online version: ./New-ServiceFabricServiceGroup.md
schema: 2.0.0
ms.assetid: 2758DDB2-A3A0-48FF-B704-4BE8FD088B5D
updated_at: 10/24/2016 10:54 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/New-ServiceFabricServiceGroupFromTemplate.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/865a3e19e58e9be5871c4d9834591e4ba1c1b9ec/Service-Fabric-cmdlets/ServiceFabric/vlatest/New-ServiceFabricServiceGroupFromTemplate.md
ms.topic: reference
ms.prod: powershell
ms.service: service-fabric
ms.technology: Azure Powershell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# New-ServiceFabricServiceGroupFromTemplate

## SYNOPSIS
Creates a Service Fabric service group from a service template.

## SYNTAX

```
New-ServiceFabricServiceGroupFromTemplate [-ApplicationName] <Uri> [-ServiceName] <Uri>
 [-ServiceTypeName] <String> [-Force] [-TimeoutSec <Int32>] [<CommonParameters>]
```

## DESCRIPTION
The **New-ServiceFabricServiceGroupFromTemplate** cmdlet creates a Service Fabric service group from the service template defined in the application manifest.

Before you perform any operation on a Service Fabric cluster, establish a connection to the cluster by using the Connect-ServiceFabricCluster cmdlet.

## EXAMPLES

### Example 1: Create a service group from a service group template
```
PS C:\>New-ServiceFabricServiceGroupFromTemplate -ApplicationName fabric:/myapp/persistenttodolist -ServiceName fabric:/myapp/persistenttodolist/svc4 -ServiceTypeName "PersistentToDoListServiceGroupType"
```

This command creates a Service Fabric service group that uses the service template for service type **PersistentToDoListServiceType**.
The type is defined in the application manifest for the fabric:/myapp/persistenttodolist Service Fabric application.

## PARAMETERS

### -ApplicationName
Specifies the Uniform Resource Identifier (URI) of a Service Fabric application.
The cmdlet creates a service group based on the application that has the URI that you specify.

```yaml
Type: Uri
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
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

### -ServiceName
Specifies the URI of a Service Fabric service group.

```yaml
Type: Uri
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ServiceTypeName
Specifies the name of a Service Fabric service group type.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
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

### None
You cannot pipe input to this cmdlet.

## OUTPUTS

### System.Object
This cmdlet returns the status of the operation as a string.

## NOTES

## RELATED LINKS

[New-ServiceFabricServiceGroup](./New-ServiceFabricServiceGroup.md)


