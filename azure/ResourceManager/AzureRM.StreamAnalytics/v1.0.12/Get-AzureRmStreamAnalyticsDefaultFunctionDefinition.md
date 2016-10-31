---
external help file: Microsoft.Azure.Commands.StreamAnalytics.dll-Help.xml
online version: .\New-AzureRmStreamAnalyticsFunction.md
schema: 2.0.0
ms.assetid: 0BBF871F-F7AE-4FEC-95ED-0629E78E681E
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.StreamAnalytics/v1.0.12/Get-AzureRmStreamAnalyticsDefaultFunctionDefinition.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.StreamAnalytics/v1.0.12/Get-AzureRmStreamAnalyticsDefaultFunctionDefinition.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureRmStreamAnalyticsDefaultFunctionDefinition

## SYNOPSIS
Gets the default definition of a function in Stream Analytics.

## SYNTAX

```
Get-AzureRmStreamAnalyticsDefaultFunctionDefinition [-JobName] <String> [-Name] <String> [-File] <String>
 [-ResourceGroupName] <String> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmStreamAnalyticsDefaultFunctionDefinition** cmdlet gets the default definition of a function in azure_2 Stream Analytics.
You can use the default definition and the New-AzureRmStreamAnalyticsFunction cmdlet to create a function.
You can modify the default definition before you create a function.

## EXAMPLES

### Example 1: Get the default definition of a Stream Analytics function
```
PS C:\>Get-AzureRmStreamAnalyticsDefaultFunctionDefinition -ResourceGroupName "StreamAnalytics-Default-West-US" -JobName "StreamJob22" -File "C:\RetrieveDefaultDefinitionRequest.json" -Name "ScoreTweet"
```

This command gets the default definition of the function named ScoreTweet by using the parameters specified in the RetrieveDefaultDefinitionRequest.json file.

## PARAMETERS

### -JobName
Specifies the name of the Stream Analytics job to which functions belong.
This cmdlet gets the default definition for a function in the job that this parameter specifies.

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

### -Name
Specifies the name of the Stream Analytics function for which this cmdlet gets the default definition.

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

### -File
Specifies the path of a .json file that contains the JavaScript Object Notation (JSON) representation of the request body for the retrieve default function definition request.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group to which Stream Analytics functions belongs.
This cmdlet gets a function definition for the group that this parameter specifies.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[New-AzureRmStreamAnalyticsFunction](xref:ResourceManager/AzureRM.StreamAnalytics/v1.0.12/New-AzureRmStreamAnalyticsFunction.md)


