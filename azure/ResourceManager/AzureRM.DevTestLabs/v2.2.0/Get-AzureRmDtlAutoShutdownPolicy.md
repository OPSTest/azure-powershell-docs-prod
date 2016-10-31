---
external help file: Microsoft.Azure.Commands.DevTestLabs.dll-Help.xml
online version: a61000e7-77e4-4441-b167-6dd304fba932
schema: 2.0.0
ms.assetid: 91E9385C-E861-4BA7-9BC9-66CEF5385CEC
updated_at: 10/28/2016 9:50 PM
ms.date: 10/28/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.DevTestLabs/v2.2.0/Get-AzureRmDtlAutoShutdownPolicy.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/e478754b524d17a2f53132d5818d405e48d9369c/azureps-cmdlets-docs/ResourceManager/AzureRM.DevTestLabs/v2.2.0/Get-AzureRmDtlAutoShutdownPolicy.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureRmDtlAutoShutdownPolicy

## SYNOPSIS
Gets the auto shutdown policy of a lab in DevTest Labs.

## SYNTAX

```
Get-AzureRmDtlAutoShutdownPolicy [-LabName] <String> [-ResourceGroupName] <String> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmDtlAutoShutdownPolicy** cmdlet gets the auto shutdown policy of a lab, which allows you to automatically shut down all the virtual machines in a lab at a specified time of the day.
The cmdlet returns whether the status of the policy is enabled, and the time of day that you have set to automatically shut down the lab virtual machines.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -LabName
Specifies the name of the lab for which this cmdlet gets the auto shutdown policy.

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
Specifies the name of the resource group that the lab belongs to.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.Azure.Commands.DevTestLabs.Models.PSSchedule
This cmdlet returns the schedule which specifies when the lab's virtual machines must shut down.

## NOTES

## RELATED LINKS

[Set-AzureRmDtlAutoShutdownPolicy](xref:ResourceManager/AzureRM.DevTestLabs/v2.2.0/Set-AzureRmDtlAutoShutdownPolicy.md)


