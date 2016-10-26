---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
online version: ./Get-ServiceFabricServiceGroupMemberType.md
schema: 2.0.0
ms.assetid: 180D2ECE-79F6-4047-99D6-5D987A90AE88
updated_at: 10/24/2016 10:54 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricServiceGroupMember.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/865a3e19e58e9be5871c4d9834591e4ba1c1b9ec/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricServiceGroupMember.md
ms.topic: reference
ms.prod: powershell
ms.service: service-fabric
ms.technology: Azure Powershell
author: visual-studio-china
ms.author: 
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-ServiceFabricServiceGroupMember

## SYNOPSIS
Gets members of service groups.

## SYNTAX

### Non-Adhoc (Default)
```
Get-ServiceFabricServiceGroupMember [-ApplicationName] <Uri> [[-ServiceName] <Uri>] [-TimeoutSec <Int32>]
 [<CommonParameters>]
```

### Adhoc
```
Get-ServiceFabricServiceGroupMember [-Adhoc] [[-ServiceName] <Uri>] [-TimeoutSec <Int32>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-ServiceFabricServiceGroupMember** cmdlet gets members of Service Fabric service groups.

Before you perform any operation on a Service Fabric cluster, establish a connection to the cluster by using the Connect-ServiceFabricCluster cmdlet.

## EXAMPLES

### Example 1: Get a service group members
```
PS C:\>Get-ServiceFabricServiceGroupMember -ApplicationName -ServiceName fabric:/CalcApp
```

The command gets Service Fabric service group members for the service named fabric:/CalcApp.

## PARAMETERS

### -Adhoc
Indicates that the service runs in ad hoc mode.
In ad hoc mode, you manually activate the service host.

```yaml
Type: SwitchParameter
Parameter Sets: Adhoc
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ApplicationName
Specifies the Uniform Resource Identifier (URI) of a Service Fabric application.
This cmdlet gets group members for the application that this parameter specifies.

```yaml
Type: Uri
Parameter Sets: Non-Adhoc
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ServiceName
Specifies the Uniform Resource Identifier (URI) of a Service Fabric service group.

```yaml
Type: Uri
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
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
This cmdlet accepts a URI that represents the name of a Service Fabric application or the name of a Service Fabric service group.

## OUTPUTS

### System.Object
This cmdlet returns a list of **System.Fabric.Query.ServiceGroupMember** objects that represent Service Fabric service group members.

## NOTES

## RELATED LINKS

[Get-ServiceFabricServiceGroupMemberType](./Get-ServiceFabricServiceGroupMemberType.md)

[New-ServiceFabricServiceGroup](./New-ServiceFabricServiceGroup.md)

[Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md)

[Get-ServiceFabricClusterConnection](./Get-ServiceFabricClusterConnection.md)


