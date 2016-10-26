---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
online version: 7370ad41-fb09-4948-9bb7-8fd67b5e99e4
schema: 2.0.0
ms.assetid: DD60B18E-5ED7-41B6-B9D4-38BD726DCFF2
updated_at: 10/24/2016 5:47 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricImageStoreContent.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/9f1d8af76684a984727546ed80c60dff01969382/Service-Fabric-cmdlets/ServiceFabric/vlatest/Get-ServiceFabricImageStoreContent.md
ms.topic: reference
ms.prod: powershell
ms.service: service-fabric
ms.technology: Azure Powershell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-ServiceFabricImageStoreContent

## SYNOPSIS
Gets content from the image store.

## SYNTAX

### Application
```
Get-ServiceFabricImageStoreContent [-Application] -ApplicationTypeName <String>
 [-ApplicationTypeVersion <String>] -ImageStoreConnectionString <String> [-TimeoutSec <Int32>]
 [<CommonParameters>]
```

### Path
```
Get-ServiceFabricImageStoreContent [-Path] [-RemoteRelativePath <String>] -ImageStoreConnectionString <String>
 [-TimeoutSec <Int32>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-ServiceFabricImageStoreContent** cmdlet gets content from the Service Fabric image store.

## EXAMPLES

### Example 1: Get image store content by application name/type
```
PS C:\>Get-ServiceFabricImageStoreContent -Application -ApplicationTypeName "CalcServiceApp" -ApplicationTypeVersion "2.0" -ImageStoreConnectionString "fabric:ImageStore"
```

This command gets image store content that belongs to the application CalcServiceApp, type version 2.0.

### Example 2: Get image store content by relative path
```
PS C:\>Get-ServiceFabricImageStoreContent -Path -RemoteRelativePath "Store\CalcServiceApp\apps" -ImageStoreConnectionString "fabric:ImageStore"
```

This command gets image store content for all application instances.

## PARAMETERS

### -Application
Indicates that image store content is searched by application type name and version.

```yaml
Type: SwitchParameter
Parameter Sets: Application
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ApplicationTypeName
Specifies the name of a Service Fabric application type.

```yaml
Type: String
Parameter Sets: Application
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ApplicationTypeVersion
Specifies the version of a Service Fabric application type version.

```yaml
Type: String
Parameter Sets: Application
Aliases: 

Required: False
Position: Named
Default value: None
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
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Path
Indicates that image store content is searched by using the image store relative path.

```yaml
Type: SwitchParameter
Parameter Sets: Path
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RemoteRelativePath
Specifies the relative path to the image store root.

```yaml
Type: String
Parameter Sets: Path
Aliases: 

Required: False
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

###  
**Get-ServiceFabricStoreContent** accepts string instances of a Service Fabric application type; the version of an application type; or the image store relative path.

## OUTPUTS

###  
**Get-ServiceFabricStoreContent** returns instances of the  **System.Fabric.Management.ImageStore.ImageStoreFile** object and/or the **System.Fabric.Management.ImageStore.ImageStoreFolder** object.

## NOTES

## RELATED LINKS


