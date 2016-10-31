---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
online version: ./Copy-ServiceFabricApplicationPackage.md
schema: 2.0.0
ms.assetid: EFDF88E2-DBFD-4868-AB66-E4F5379C55A9
updated_at: 10/24/2016 10:54 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Remove-ServiceFabricApplicationPackage.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/865a3e19e58e9be5871c4d9834591e4ba1c1b9ec/Service-Fabric-cmdlets/ServiceFabric/vlatest/Remove-ServiceFabricApplicationPackage.md
ms.topic: reference
ms.prod: powershell
ms.service: service-fabric
ms.technology: Azure Powershell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Remove-ServiceFabricApplicationPackage

## SYNOPSIS
Removes a Service Fabric application package from the image store.

## SYNTAX

```
Remove-ServiceFabricApplicationPackage [-ApplicationPackagePathInImageStore] <String>
 [-ImageStoreConnectionString] <String> [-TimeoutSec <Int32>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-ServiceFabricApplicationPackage** cmdlet removes a Service Fabric application package from the image store.
Run this cmdlet after you register the application package by using the **Register-ServiceFabricApplicationPackage** cmdlet.

To manage Service Fabric clusters, start Windows PowerShell by using the Run as administrator option.
Before you perform any operation on a Service Fabric cluster, establish a connection to the cluster by using the Connect-ServiceFabricCluster cmdlet.

## EXAMPLES

### Example 1: Remove an application package
```
PS C:\>Remove-ServiceFabricApplicationPackage -ImageStoreConnectionString "xstore:DefaultEndpointsProtocol=https;AccountName=[StorageAccountName];AccountKey=[StorageAccountKey];Container=[ContainerName]" -ApplicationPackagePathInImageStore "PersistentToDoListService_v2"
```

This command removes the application package that has the specified image store path.
The cmdlet does prompt you for confirmation before it removes the application package.

## PARAMETERS

### -ApplicationPackagePathInImageStore
Specifies the relative path in the image store.
The cmdlet removes the package from the path that this parameter specifies.

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

### -ImageStoreConnectionString
Specifies the connection string for the Service Fabric image store.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
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

[Copy-ServiceFabricApplicationPackage](xref:ServiceFabric/vlatest/Copy-ServiceFabricApplicationPackage.md)

[Test-ServiceFabricApplicationPackage](xref:ServiceFabric/vlatest/Test-ServiceFabricApplicationPackage.md)


