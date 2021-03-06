---
external help file: Microsoft.Azure.Commands.Insights.dll-Help.xml
ms.assetid: A837077C-0A79-431C-93D2-799B2134EE69
online version: 
schema: 2.0.0
updated_at: 1/11/2017 9:26 PM
ms.date: 1/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Insights/v2.4.0/Get-AzureRmAlertRule.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Insights/v2.4.0/Get-AzureRmAlertRule.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/cf5fb15dcd1fe2c86458f47e1a11dc88817021fc/azureps-cmdlets-docs/ResourceManager/AzureRM.Insights/v2.4.0/Get-AzureRmAlertRule.md
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

# Get-AzureRmAlertRule

## SYNOPSIS
Gets alert rules.

## SYNTAX

### Parameters for Get-AzureRmAlertRule cmdlet
```
Get-AzureRmAlertRule -ResourceGroup <String> [-DetailedOutput] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

### Parameters for Get-AzureRmAlertRule cmdlet using name
```
Get-AzureRmAlertRule -ResourceGroup <String> -Name <String> [-DetailedOutput]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

### Parameters for Get-AzureRmAlertRule cmdlet using target resource uri
```
Get-AzureRmAlertRule -ResourceGroup <String> -TargetResourceId <String> [-DetailedOutput]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmAlertRule** cmdlet gets an alert rule by its name or URI, or all alert rules from a specified resource group.

## EXAMPLES

### Example 1: Get alert rules for a resource group
```
PS C:\>Get-AzureRmAlertRule -ResourceGroup "Default-Web-CentralUS"
```

This command gets all of the alert rules for the resource group named Default-Web-CentralUS.
The output does not contain details about the rules because the *DetailedOutput* parameter is not specified.

### Example 2: Get an alert rule by name
```
PS C:\>Get-AzureRmAlertRule -ResourcGroup "Default-Web-CentralUS" -Name "myalert-7da64548-214d-42ca-b12b-b245bb8f0ac8"
```

This command gets the alert rule named myalert-7da64548-214d-42ca-b12b-b245bb8f0ac8.
Because the *DetailedOutput* parameter is not specified, the output contains only basic information about the alert rule.

### Example 3: Get an alert rule by name with detailed output
```
PS C:\>Get-AzureRmAlertRule -ResourceGroup "Default-Web-CentralUS" -Name "myalert-7da64548-214d-42ca-b12b-b245bb8f0ac8" -DetailedOutput
```

This command gets the alert rule named myalert-7da64548-214d-42ca-b12b-b245bb8f0ac8.
The *DetailedOutput* parameter is specified, so the output is detailed.

## PARAMETERS

### -DetailedOutput
Displays full details in the output.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -InformationAction
@{Text=}```yaml
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
@{Text=}```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the name of the alert rule to get.

```yaml
Type: String
Parameter Sets: Parameters for Get-AzureRmAlertRule cmdlet using name
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroup
Specifies the name of the resource group.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -TargetResourceId
Specifies the ID of the target resource.

```yaml
Type: String
Parameter Sets: Parameters for Get-AzureRmAlertRule cmdlet using target resource uri
Aliases: 

Required: True
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

[Add-AzureRmLogAlertRule](xref:ResourceManager/AzureRM.Insights/v2.4.0/Add-AzureRmLogAlertRule.md)

[Add-AzureRmMetricAlertRule](xref:ResourceManager/AzureRM.Insights/v2.4.0/Add-AzureRmMetricAlertRule.md)

[Add-AzureRmWebtestAlertRule](xref:ResourceManager/AzureRM.Insights/v2.4.0/Add-AzureRmWebtestAlertRule.md)

[Get-AzureRmAlertHistory](xref:ResourceManager/AzureRM.Insights/v2.4.0/Get-AzureRmAlertHistory.md)

[Remove-AzureRmAlertRule](xref:ResourceManager/AzureRM.Insights/v2.4.0/Remove-AzureRmAlertRule.md)


