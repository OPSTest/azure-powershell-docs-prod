---
external help file: Microsoft.Azure.Commands.Batch.dll-Help.xml
ms.assetid: A39A415A-B403-48D3-AF80-CF7CFE382577
online version: 
schema: 2.0.0
updated_at: 11/17/2016 12:05 AM
ms.date: 11/17/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Batch/v2.3.0/Get-AzureRmBatchLocationQuotas.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Batch/v2.3.0/Get-AzureRmBatchLocationQuotas.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/e571c04f9a934d1d758a5e8cee0c6c5b87856e76/azureps-cmdlets-docs/ResourceManager/AzureRM.Batch/v2.3.0/Get-AzureRmBatchLocationQuotas.md
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

# Get-AzureRmBatchLocationQuotas

## SYNOPSIS
Gets the Batch service quotas for your subscription at the given location.

## SYNTAX

```
Get-AzureRmBatchLocationQuotas [-Location] <String>
```

## DESCRIPTION
Gets the Batch service quotas for the specified subscription at the given location.

## EXAMPLES

### Example 1: Get the Batch service quotas for the subscription in the West US region 

```
PS C:\>Get-AzureRmBatchLocationQuotas -Location "westus"
          AccountQuota Location
          ------------ --------
          1            westus
```

This command gets the quotas for the current subscription in the West US region.
The return value indicates that this subscription can create only one Batch account in that region.

## PARAMETERS

### -Location
Specifies the region for which this cmdlet checks the quotas.
For more information, see Azure Regions (https://azure.microsoft.com/regions).

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

## INPUTS

## OUTPUTS

### Microsoft.Azure.Commands.Batch.Models.PSBatchLocationQuotas

## NOTES

## RELATED LINKS


