---
external help file: Microsoft.Azure.Commands.Insights.dll-Help.xml
online version: 7b6e8604-1bf0-4256-a37f-889743fe9fcd
schema: 2.0.0
ms.assetid: 219D5A7F-E37C-4F37-AFC1-61C17680E25A
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Insights/v2.2.0/Get-AzureRmUsage.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Insights/v2.2.0/Get-AzureRmUsage.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: 
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureRmUsage

## SYNOPSIS
Gets the usage metrics for a resource.

## SYNTAX

```
Get-AzureRmUsage [-ResourceId] <String> [-ApiVersion <String>] [-StartTime <DateTime>] [-EndTime <DateTime>]
 [-MetricNames <String[]>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmUsage** cmdlet gets the usage metrics for a specified resource.

## EXAMPLES

### Example 1: Get usage metrics by resource ID
```
PS C:\>Get-AzureRmUsage -ResourceId "/subscriptions/bcdeb07f-1c43-20be-1f3b-4f0febc10f5b/resourceGroups/Default-Web-EastUS/providers/microsoft.web/sites/pattifuller"
```

This command gets the usage metrics for the specified website.

## PARAMETERS

### -ResourceId
Specifies the ID of the resource for the metric.

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

### -ApiVersion
Specifies an API version string, for example, 2014-04-01, which is accepted by the resource provider.

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

### -StartTime
Specifies the earliest time and date to search.

You can use the Get-Date cmdlet to get a **DateTime** object.

```yaml
Type: DateTime
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -EndTime
Specifies the latest time and date to search.

You can use the Get-Date cmdlet to get a **DateTime** object.

```yaml
Type: DateTime
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -MetricNames
Specifies an array of names of metrics.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
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

[Get-AzureRmMetric](xref:ResourceManager/AzureRM.Insights/v2.2.0/Get-AzureRmMetric.md)


