---
external help file: Microsoft.Azure.Commands.Batch.dll-Help.xml
ms.assetid: B423C1A1-1988-4721-81E7-3B7EC163B03A
online version: 
schema: 2.0.0
updated_at: 1/20/2017 9:17 PM
ms.date: 1/20/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Batch/v2.5.0/New-AzureBatchCertificate.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Batch/v2.5.0/New-AzureBatchCertificate.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/cb06bb906911a2a2e1f57adbafe0c0c97a0b205b/azureps-cmdlets-docs/ResourceManager/AzureRM.Batch/v2.5.0/New-AzureBatchCertificate.md
ms.topic: reference
ms.prod: powershell
ms.technology: Azure PowerShell
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: False
ms.service: azure-powershell
---

# New-AzureBatchCertificate

## SYNOPSIS
Adds a certificate to the specified Batch account.

## SYNTAX

### File (Default)
```
New-AzureBatchCertificate [-FilePath] <String> [-Password <String>] -BatchContext <BatchAccountContext>
 [<CommonParameters>]
```

### RawData
```
New-AzureBatchCertificate [-RawData] <Byte[]> [-Password <String>] -BatchContext <BatchAccountContext>
 [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureBatchCertificate** cmdlet adds a certificate to the specified Azure Batch account.

## EXAMPLES

### Example 1: Add a certificate from a file
```
PS C:\>New-AzureBatchCertificate -FilePath "E:\Certificates\MyCert.cer" -BatchContext $Context
```

This command adds a certificate to the specified Batch account by using the file E:\Certificates\MyCert.cer.

### Example 2: Add a certificate from raw data
```
PS C:\>$RawData = [System.IO.File]::ReadAllBytes("E:\Certificates\MyCert.pfx")
PS C:\> New-AzureBatchCertificate -RawData $RawData -Password "Password1234" -BatchContext $Context
```

The first command reads the data from the file named MyCert.pfx into the $RawData variable.

The second command adds a certificate to the specified Batch account using the raw data stored in $RawData.

## PARAMETERS

### -BatchContext
Specifies the **BatchAccountContext** instance that this cmdlet uses to interact with the Batch service.
To obtain a **BatchAccountContext** object that contains access keys for your subscription, use the Get-AzureRmBatchAccountKeys cmdlet.

```yaml
Type: BatchAccountContext
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -FilePath
Specifies the path of the certificate file.
The certificate file must be in either .cer or .pfx format.

```yaml
Type: String
Parameter Sets: File
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Password
Specifies the password to access the certificate private key.
You must specify this parameter if you specify a certificate in .pfx format.

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

### -RawData
Specifies the raw certificate data in either .cer or .pfx format.

```yaml
Type: Byte[]
Parameter Sets: RawData
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureBatchCertificate](xref:ResourceManager/AzureRM.Batch/v2.5.0/Get-AzureBatchCertificate.md)

[Get-AzureRmBatchAccountKeys](xref:ResourceManager/AzureRM.Batch/v2.5.0/Get-AzureRmBatchAccountKeys.md)

[Remove-AzureBatchCertificate](xref:ResourceManager/AzureRM.Batch/v2.5.0/Remove-AzureBatchCertificate.md)

[Azure Batch Cmdlets](xref:ResourceManager/AzureRM.Batch/v2.5.0/AzureRM.Batch.md)


