---
external help file: Microsoft.WindowsAzure.Commands.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 73AA8912-EFA3-4FEA-8AEC-402B7C0BFA92
updated_at: 11/1/2016 10:24 PM
ms.date: 11/1/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v3.0.0/Get-AzureSchedulerLocation.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/f59f3ef60bc592383812213e69fd77ba950759ed/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v3.0.0/Get-AzureSchedulerLocation.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: ServiceManagement_Azure_Compute_v3_0_0_Get_AzureSchedulerLocation_md
---

# Get-AzureSchedulerLocation

## SYNOPSIS
Gets available scheduler locations.

## SYNTAX

```
Get-AzureSchedulerLocation [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
This topic describes the cmdlet in the 0.8.10 version of the Microsoft Azure PowerShell module.
To get the version of the module you're using, in the Azure PowerShell console, type (Get-Module -Name Azure).Version.

The **Get-AzureSchedulerLocation** cmdlet gets available scheduler locations.

## EXAMPLES

### Example 1: Get available scheduler locations
```
PS C:\>Get-AzureSchedulerLocation
```

This command gets available scheduler locations.

## PARAMETERS

### -Profile
Specifies the Azure profile from which this cmdlet reads.
If you do not specify a profile, this cmdlet reads from the local default profile.

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

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureSchedulerJob](xref:ServiceManagement/Azure.Compute/v3.0.0/Get-AzureSchedulerJob.md)

[Get-AzureSchedulerJobCollection](xref:ServiceManagement/Azure.Compute/v3.0.0/Get-AzureSchedulerJobCollection.md)

[Get-AzureSchedulerJobHistory](xref:ServiceManagement/Azure.Compute/v3.0.0/Get-AzureSchedulerJobHistory.md)


