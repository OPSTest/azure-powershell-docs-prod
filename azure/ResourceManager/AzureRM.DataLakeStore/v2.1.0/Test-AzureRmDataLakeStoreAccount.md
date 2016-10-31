---
external help file: Microsoft.Azure.Commands.DataLakeStore.dll-Help.xml
online version: .\Get-AzureRmDataLakeStoreAccount.md
schema: 2.0.0
ms.assetid: 70CBDDFB-CACD-4500-837B-FF3F11C99E1F
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.DataLakeStore/v2.1.0/Test-AzureRmDataLakeStoreAccount.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.DataLakeStore/v2.1.0/Test-AzureRmDataLakeStoreAccount.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: 
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Test-AzureRmDataLakeStoreAccount

## SYNOPSIS
Tests the existence of a Data Lake Store account.

## SYNTAX

```
Test-AzureRmDataLakeStoreAccount [-Name] <String> [[-ResourceGroupName] <String>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Test-AzureRmDataLakeStoreAccount** cmdlet tests the existence of a Data Lake Store account.

## EXAMPLES

### Example 1: Test an account
```
PS C:\>Test-AzureRmDataLakeStoreAccount -Name "ContosoADL"
```

This command tests whether the account named ContosoADL exists.

## PARAMETERS

### -Name
Specifies the name of the Data Lake Store account to test.

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

### -ResourceGroupName
Specifies the name of the resource group that contains the account to test.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -InformationAction
@{Text=}

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
@{Text=}

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmDataLakeStoreAccount](xref:ResourceManager/AzureRM.DataLakeStore/v2.1.0/Get-AzureRmDataLakeStoreAccount.md)

[New-AzureRmDataLakeStoreAccount](xref:ResourceManager/AzureRM.DataLakeStore/v2.1.0/New-AzureRmDataLakeStoreAccount.md)

[Remove-AzureRmDataLakeStoreAccount](xref:ResourceManager/AzureRM.DataLakeStore/v2.1.0/Remove-AzureRmDataLakeStoreAccount.md)

[Set-AzureRmDataLakeStoreAccount](xref:ResourceManager/AzureRM.DataLakeStore/v2.1.0/Set-AzureRmDataLakeStoreAccount.md)


