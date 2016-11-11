---
external help file: Microsoft.AzureStack.Commands.dll-Help.xml
online version: 
schema: 2.0.0
updated_at: 11/5/2016 1:26 AM
ms.date: 11/5/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.AzureStackAdmin/v1.2.6/Add-AzureRMUsageConnection.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/575d9503d8b0c84528eba60a4cccb3d04eac677d/azureps-cmdlets-docs/ResourceManager/AzureRM.AzureStackAdmin/v1.2.6/Add-AzureRMUsageConnection.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: ResourceManager_AzureRM_AzureStackAdmin_v1_2_6_Add_AzureRMUsageConnection_md
---

# Add-AzureRMUsageConnection

## SYNOPSIS
The Add-AzureRMUsageConnection cmdlet adds an usage connection details for a resource provider.
The cmdlet gets the storage account information where the resource provider is storing the usage records.
This information is given to the usage service through this cmdlet. 
Usage Service will retrieve the usage records periodically from the storage account information provided

## SYNTAX

```
Add-AzureRMUsageConnection -Name <String> -ResourceGroup <String> [-SubscriptionId <Guid>]
 -ArmLocation <String> -ProviderLocation <String> -ProviderNamespace <String>
 -UsageStorageConnectionString <String> -UsageReportingQueue <String> -UsageReportingTable <String>
 -ErrorReportingQueue <String> -ErrorReportingTable <String> [-AdminUri <Uri>] [-Token <String>]
 [-ApiVersion <String>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [-PipelineVariable <String>]
```

## DESCRIPTION

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
Add-AzureRmUsageConnection @usageConnectionParams
```

Description

-----------

The following example registers a usage connection information of a resource provider to usage service

            $usageConnectionId = "sqlrpusageconnection"
            $location = "local"

            # Create Resource Group
            # The following name could be anything
            $usageConnectionRG="UsageConnectionRG"
            New-AzureRMResourceGroup -Name $usageConnectionRG  -Location $location -Force

            # Make sure the tables and queues exist
            # if not create them with New-AzureStorageTale/New-AzureStorageQueue
            $usageReportingQueue = "sqlrpusagequeue"
            $usageReportingTable = "sqlrpusagetable"
            $errorReportingQueue = "sqlrpusageerrorqueue"
            $errorReportingTable = "sqlrpusageerrortable"

            # Create Storage Account If Other than DevStorage
            $storageConnectionString = "UseDevelopmentStorage=true"


            $usageConnectionParams = @{
            Name = $usageConnectionId
            ResourceGroup = $usageConnectionRG
            ProviderNamespace = "Microsoft.Sql"
            ArmLocation = $location
            ProviderLocation = $location
            UsageStorageConnectionString = $storageConnectionString
            UsageReportingQueue = $usageReportingQueue
            UsageReportingTable = $usageReportingTable
            ErrorReportingQueue = $errorReportingQueue
            ErrorReportingTable = $errorReportingTable
            ApiVersion = "2015-06-01-preview"
            }

            Add-AzureRmUsageConnection @usageConnectionParams

## PARAMETERS

### -AdminUri
Specifies the azure stack resource manager endpoint.
This parameter is not needed when using the cmdlet against the azure stack environment configured against azure active directory

```yaml
Type: Uri
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ApiVersion
API Version for the usage connection api.
This needs to be '2015-06-01-preview' .
Note that this parameter will get removed in a future release

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ArmLocation
This is the Location of the resource manager instance in the Azure Stack installation

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

### -ErrorReportingQueue
Queue name for reporting the errors.
Usage service would insert records in this queue for any errors during its collection process

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ErrorReportingTable
Table name for reporting the errors.
Usage service would insert records in this queue for any errors during its collection process

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -InformationAction
Not Specified

The following values are permitted for this object type.

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa
Accepted values: SilentlyContinue, Stop, Continue, Inquire

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
Not Specified

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the name of the usage connection

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PipelineVariable
Not Specified

```yaml
Type: String
Parameter Sets: (All)
Aliases: pv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ProviderLocation
Location of the resource provider for which the usage connection is being added

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ProviderNamespace
Namespace of the resource provider for which the usage connection is being added

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroup
Resource group name for the usage connection resource

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -SubscriptionId
Service administrator subscription id.
This parameter is not needed when using the cmdlet against the azure stack environment configured against azure active directory. 
This parameter will be deprecated in a future release

```yaml
Type: Guid
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Token
Authentication token for making the request.
This parameter is not needed when using the cmdlet against the azure stack environment configured against azure active directory. 
This parameter will be deprecated in a future release

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -UsageReportingQueue
Queue name where the added usage meta data is queued .
Using this metadata, Usage service will read the data from reporting table for usage aggregation

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -UsageReportingTable
Table name where usage records are inserted

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -UsageStorageConnectionString
This specifies the storage connection string in which the resource provider usage records are inserted

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

### Microsoft.AzureStack.Management.Models.UsageConnectionModel

## NOTES
## RELATED LINKS

