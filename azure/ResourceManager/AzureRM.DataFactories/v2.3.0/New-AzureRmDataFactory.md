---
external help file: Microsoft.Azure.Commands.DataFactories.dll-Help.xml
ms.assetid: FAFA8304-D8D2-459C-86D7-7DA0E1D30012
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.DataFactories/v2.3.0/New-AzureRmDataFactory.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.DataFactories/v2.3.0/New-AzureRmDataFactory.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# New-AzureRmDataFactory

## SYNOPSIS
Creates a data factory.

## SYNTAX

```
New-AzureRmDataFactory [-Name] <String> [-Location] <String> [[-Tags] <Hashtable>] [-Force]
 [-ResourceGroupName] <String> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureRmDataFactory** cmdlet creates a data factory with the specified resource group name and location.

Perform these operations in the following order: 

- Create a data factory. 
- Create linked services. 
- Create datasets. 
- Create a pipeline.

## EXAMPLES

### Example 1: Create a data factory
```
PS C:\>New-AzureRmDataFactory -ResourceGroupName "ADF" -Name "WikiADF" -Location "WestUS"
DataFactoryName   : WikiADF
ResourceGroupName : ADF
Location          : WestUS
Tags              : {}
Properties        : Microsoft.WindowsAzure.Commands.Utilities.PSDataFactoryConfiguration
```

This command creates a data factory named WikiADF in the resource group named ADF in the WestUS location.

## PARAMETERS

### -Force
Indicates that this cmdlet replaces an existing data factory without prompting you for confirmation.

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

### -Location
Specifies the location for the data factory, such as WestUS or EastUS.
Only WestUS is currently supported.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the name of the data factory to create.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of an Azure resource group.
This cmdlet creates a data factory that belongs to the group that this parameter specifies.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Tags
Specifies tags for the data factory.

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases: 

Required: False
Position: 4
Default value: None
Accept pipeline input: True (ByPropertyName)
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

## OUTPUTS

### Microsoft.WindowsAzure.Commands.Utilities.PSDataFactory

## NOTES
* Keywords: azure, azurerm, arm, resource, management, manager, data, factories

## RELATED LINKS

[Get-AzureRmDataFactory](xref:ResourceManager/AzureRM.DataFactories/v2.3.0/Get-AzureRmDataFactory.md)

[Remove-AzureRmDataFactory](xref:ResourceManager/AzureRM.DataFactories/v2.3.0/Remove-AzureRmDataFactory.md)

