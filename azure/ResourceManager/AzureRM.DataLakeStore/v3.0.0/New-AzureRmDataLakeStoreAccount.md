---
external help file: Microsoft.Azure.Commands.DataLakeStore.dll-Help.xml
online version: 5007baf3-b84b-44cf-9dcd-12f0f712d9bd
schema: 2.0.0
ms.assetid: 1E2DAAE8-EB5B-490F-AB29-28B588D1141B
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.DataLakeStore/v3.0.0/New-AzureRmDataLakeStoreAccount.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.DataLakeStore/v3.0.0/New-AzureRmDataLakeStoreAccount.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: 
keywords: powershell, cmdlet
manager: visual-studio-china
---

# New-AzureRmDataLakeStoreAccount

## SYNOPSIS
Creates a new Data Lake Store account.

## SYNTAX

```
New-AzureRmDataLakeStoreAccount [-ResourceGroupName] <String> [-Name] <String> [-Location] <String>
 [[-DefaultGroup] <String>] [[-Tags] <Hashtable>] [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureRmDataLakeStoreAccount** cmdlet creates a new Data Lake Store account.

## EXAMPLES

### Example 1: Create an account
```
PS C:\>New-AzureRmDataLakeStoreAccount -Name "ContosoADL" -ResourceGroupName "ContosoOrg" -Location "East US 2"
```

This command creates a Data Lake Store account named ContosoADL for the East US 2 location.

## PARAMETERS

### -ResourceGroupName
Specifies the name of the resource group that contains the account.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the name of the account to create.

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

### -Location
Specifies the location to use for the account.
The acceptable values for this parameter are:

- East US 2

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

### -DefaultGroup
Specifies the object ID of the AzureActive Directory group to use as the default group owner for new files and folders.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Tags
Specifies tags as key-value pairs.
You can use tags to identify a Data Lake Store account from other Azure resources.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmDataLakeStoreAccount](xref:ResourceManager/AzureRM.DataLakeStore/v3.0.0/Get-AzureRmDataLakeStoreAccount.md)

[Remove-AzureRmDataLakeStoreAccount](xref:ResourceManager/AzureRM.DataLakeStore/v3.0.0/Remove-AzureRmDataLakeStoreAccount.md)

[Set-AzureRmDataLakeStoreAccount](xref:ResourceManager/AzureRM.DataLakeStore/v3.0.0/Set-AzureRmDataLakeStoreAccount.md)

[Test-AzureRmDataLakeStoreAccount](xref:ResourceManager/AzureRM.DataLakeStore/v3.0.0/Test-AzureRmDataLakeStoreAccount.md)


