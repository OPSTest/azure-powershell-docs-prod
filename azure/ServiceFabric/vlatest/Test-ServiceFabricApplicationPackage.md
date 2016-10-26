---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
online version: ./Connect-ServiceFabricCluster.md
schema: 2.0.0
ms.assetid: 81C3B5F4-6B48-47CB-AC09-3193F3F86E25
updated_at: 10/24/2016 10:54 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Test-ServiceFabricApplicationPackage.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/865a3e19e58e9be5871c4d9834591e4ba1c1b9ec/Service-Fabric-cmdlets/ServiceFabric/vlatest/Test-ServiceFabricApplicationPackage.md
ms.topic: reference
ms.prod: powershell
ms.service: service-fabric
ms.technology: Azure Powershell
author: visual-studio-china
ms.author: 
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Test-ServiceFabricApplicationPackage

## SYNOPSIS
Validates a Service Fabric application package.

## SYNTAX

```
Test-ServiceFabricApplicationPackage [-ApplicationPackagePath] <String> [-ApplicationParameter <Hashtable>]
 [-ImageStoreConnectionString <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Test-ServiceFabricApplicationPackage** cmdlet validates a Service Fabric application package.
After you validate a package, use the Copy-ServiceFabricApplicationPackage cmdlet to copy it to the image store.

Before you perform any operation on a Service Fabric cluster, establish a connection to the cluster by using the Connect-ServiceFabricCluster cmdlet.

## EXAMPLES

### Example 1: Validate a package
```
PS C:\>Test-ServiceFabricApplicationPackage -ApplicationPackagePath "C:\PersistentToDoListService"
```

This command validates the application package in the specified path.

## PARAMETERS

### -ApplicationPackagePath
Specifies the relative path of an application package.
The cmdlet validates the package in the path that you specify.

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

### -ApplicationParameter
Specifies the overrides for application parameters as name/value pairs.

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ImageStoreConnectionString
Specifies the connection string for the Service Fabric image store.
If you specify this parameter, the cmdlet performs additional validations against previously deployed versions currently in the store.

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
This cmdlet returns $True if the Service Fabric application package is valid, or, if it is not valid, this cmdlet returns $False.

## NOTES

## RELATED LINKS

[Connect-ServiceFabricCluster](./Connect-ServiceFabricCluster.md)

[Copy-ServiceFabricApplicationPackage](./Copy-ServiceFabricApplicationPackage.md)

[Get-ServiceFabricClusterConnection](./Get-ServiceFabricClusterConnection.md)

[Remove-ServiceFabricApplicationPackage](./Remove-ServiceFabricApplicationPackage.md)


