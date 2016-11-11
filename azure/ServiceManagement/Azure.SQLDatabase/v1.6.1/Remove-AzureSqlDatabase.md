---
external help file: Microsoft.WindowsAzure.Commands.SqlDatabase.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: F4CB9D02-EAA6-4C6B-8532-DB8E95E69A3E
updated_at: 11/1/2016 10:24 PM
ms.date: 11/1/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ServiceManagement/Azure.SQLDatabase/v1.6.1/Remove-AzureSqlDatabase.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/f59f3ef60bc592383812213e69fd77ba950759ed/azureps-cmdlets-docs/ServiceManagement/Azure.SQLDatabase/v1.6.1/Remove-AzureSqlDatabase.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: ServiceManagement_Azure_SQLDatabase_v1_6_1_Remove_AzureSqlDatabase_md
---

# Remove-AzureSqlDatabase

## SYNOPSIS
Deletes an ssSDS.

## SYNTAX

### ByObjectWithConnectionContext
```
Remove-AzureSqlDatabase [-ConnectionContext] <IServerDataServiceContext> [-Database] <Database> [-Force]
 [-Profile <AzureSMProfile>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### ByNameWithConnectionContext
```
Remove-AzureSqlDatabase [-ConnectionContext] <IServerDataServiceContext> [-DatabaseName] <String> [-Force]
 [-Profile <AzureSMProfile>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

### ByNameWithServerName
```
Remove-AzureSqlDatabase [-ServerName] <String> [-DatabaseName] <String> [-Force] [-Profile <AzureSMProfile>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### ByObjectWithServerName
```
Remove-AzureSqlDatabase [-ServerName] <String> [-Database] <Database> [-Force] [-Profile <AzureSMProfile>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureSqlDatabase** cmdlet deletes an ssSDS by server connection context or server name.
You can create an ssSDS server connection context using the New-AzureSqlDatabaseServerContext cmdlet, and then use it with this cmdlet.

When you delete a database by specifying an ssSDS server name, the **Remove-AzureSqlDatabase** cmdlet uses the name and the current Azure subscription information to perform the operation.

## EXAMPLES

### Example 1: Remove a database
```
PS C:\>Remove-AzureSqlDatabase -ConnectionContext $Context -DatabaseName "Database01"
```

This command removes the database named Database01 from the ssSDS server connection context $Context.

### Example 2: Remove a database by using a server name
```
PS C:\>Remove-AzureSqlDatabase -ServerName "lpqd0zbr8y" -DatabaseName "Database01"
```

This command removes the database named Database01 from the ssSDS server namedlpqd0zbr8y.

### Example 3: Remove a database by using the pipeline
```
PS C:\>$Database01 | Remove-AzureSqlDatabase -ConnectionContext $Context
PS C:\> $Database01 | Remove-AzureSqlDatabase -ServerName "lpqd0zbr8y"
```

This example demonstrates the alternative method of passing the database object through the pipeline.

## PARAMETERS

### -ConnectionContext
Specifies the connection context of a server from which this cmdlet removes a database.

```yaml
Type: IServerDataServiceContext
Parameter Sets: ByObjectWithConnectionContext, ByNameWithConnectionContext
Aliases: Context

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Database
Specifies an object that represents the database that this cmdlet removes.

```yaml
Type: Database
Parameter Sets: ByObjectWithConnectionContext, ByObjectWithServerName
Aliases: InputObject

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Force
Allows the action to complete without prompting the user for confirmation.

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

### -WhatIf
Shows what would happen if the cmdlet runs.
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

### -Confirm
Prompts you for confirmation before running the cmdlet.

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

### -DatabaseName
Specifies the name of the database that this cmdlet removes.

```yaml
Type: String
Parameter Sets: ByNameWithConnectionContext, ByNameWithServerName
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ServerName
Specifies the name of the server on which this cmdlet deletes the database.

```yaml
Type: String
Parameter Sets: ByNameWithServerName, ByObjectWithServerName
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

## OUTPUTS

## NOTES
* Because of the severity of the operation, by default, this cmdlet prompts you for confirmation. To skip confirmation, specify the *Force* parameter.

## RELATED LINKS

[Azure SQL Database](https://azure.microsoft.com/en-us/services/sql-database/)

[Delete Database](https://msdn.microsoft.com/en-us/library/azure/dn505705.aspx)

[Operations for Azure SQL Databases](https://msdn.microsoft.com/en-us/library/azure/dn505719.aspx)

[Get-AzureSqlDatabase](xref:ServiceManagement/Azure.SQLDatabase/v1.6.1/Get-AzureSqlDatabase.md)

[New-AzureSqlDatabase](xref:ServiceManagement/Azure.SQLDatabase/v1.6.1/New-AzureSqlDatabase.md)

[New-AzureSqlDatabaseServerContext](xref:ServiceManagement/Azure.SQLDatabase/v1.6.1/New-AzureSqlDatabaseServerContext.md)

[Set-AzureSqlDatabase](xref:ServiceManagement/Azure.SQLDatabase/v1.6.1/Set-AzureSqlDatabase.md)


