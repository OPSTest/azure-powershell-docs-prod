---
external help file: Microsoft.WindowsAzure.Commands.SqlDatabase.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: C75C29A7-A26A-4D75-B068-C5440F2C1158
updated_at: 11/11/2016 11:03 PM
ms.date: 11/11/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ServiceManagement/Azure.SQLDatabase/v1.6.1/Get-AzureSqlDatabaseOperation.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/79eeb985ea480979357fb4695832a0c3d29a48bf/azureps-cmdlets-docs/ServiceManagement/Azure.SQLDatabase/v1.6.1/Get-AzureSqlDatabaseOperation.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: ServiceManagement_Azure_SQLDatabase_v1_6_1_Get_AzureSqlDatabaseOperation_md
---

# Get-AzureSqlDatabaseOperation

## SYNOPSIS
Gets the status of database operations on an Azure server.

## SYNTAX

### ByConnectionContext (Default)
```
Get-AzureSqlDatabaseOperation [-ConnectionContext] <IServerDataServiceContext> [-Database <Database>]
 [-DatabaseName <String>] [-OperationGuid <Guid>] [-Profile <AzureSMProfile>] [<CommonParameters>]
```

### ByServerName
```
Get-AzureSqlDatabaseOperation [-ServerName] <String> [-Database <Database>] [-DatabaseName <String>]
 [-OperationGuid <Guid>] [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureSqlDatabaseOperation** cmdlet gets the status of database operations on the specified Azure server.
If you specify only the *ServerName* or *ConnectionContext* parameter, the cmdlet gets all the database operations for the server.
If you also specify a database by using the *Database* or *DatabaseName* parameter, this cmdlet gets all the operations for the specified database.
If you specify an operation GUID, and *ServerName* or *ConnectionContext*, the cmdlet gets a single database operation.

## EXAMPLES

### Example 1: Get the status of all database operations for a database
```
PS C:\>$Operations = Get-AzureSqlDatabaseOperation -ConnectionContext $Context -DatabaseName "Database17"
```

This command gets the status of all database operations on the database named Database17 on the server that the connection context $Context specifies.

### Example 2: Get the status of all database operations for a server
```
PS C:\>$Operations = Get-AzureSqlDatabaseOperation -ConnectionContext $Context
```

This command gets the status of all database operations on the server that the connection context $Context specifies.

## PARAMETERS

### -ConnectionContext
Specifies the connection context of a server.

```yaml
Type: IServerDataServiceContext
Parameter Sets: ByConnectionContext
Aliases: Context

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Database
Specifies an object that represents an ssSDS.
If you specify this parameter, you must specify the *ServerName* parameter or *ConnectionContext* parameter.

```yaml
Type: Database
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -DatabaseName
Specifies the name of a database.
If you specify this parameter, you must specify the *ServerName* parameter or the *ConnectionContext* parameter.

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

### -OperationGuid
Specifies the operation ID that represents a specific database operation for which this cmdlet gets status.
You can obtain operation IDs by requesting all the database operations for a ssSDS or server.
If you specify this parameter, you must specify the *ServerName* parameter or the *ConnectionContext* parameter.

```yaml
Type: Guid
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -ServerName
Specifies the name of a server.

```yaml
Type: String
Parameter Sets: ByServerName
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Profile
ps_azureprofile_description

```yaml
Type: AzureSMProfile
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

### Microsoft.WindowsAzure.Commands.SqlDatabase.Services.Server.Database

### Microsoft.WindowsAzure.Commands.SqlDatabase.Model.SqlDatabaseServerContext

### System.Guid

## OUTPUTS

### Microsoft.WindowsAzure.Commands.SqlDatabase.Services.Server.Database.DatabaseOperationResponseList[]
This cmdlet returns an array of **DatabaseOperationResponseList** objects if you get multiple operations.

### Microsoft.WindowsAzure.Commands.SqlDatabase.Services.Server.Database.DatabaseOperationResponse

## NOTES

## RELATED LINKS

[Azure SQL Database](http://msdn.microsoft.com/library/ee336279.aspx)

[Database Operation Status](https://msdn.microsoft.com/en-us/library/azure/dn720371.aspx)

[Operations for Azure SQL Databases](https://msdn.microsoft.com/en-us/library/azure/dn505719.aspx)

[Get-AzureSqlDatabase](xref:ServiceManagement/Azure.SQLDatabase/v1.6.1/Get-AzureSqlDatabase.md)

[New-AzureSqlDatabaseServerContext](xref:ServiceManagement/Azure.SQLDatabase/v1.6.1/New-AzureSqlDatabaseServerContext.md)


