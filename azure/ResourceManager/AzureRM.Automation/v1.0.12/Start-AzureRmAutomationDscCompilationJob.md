---
external help file: Microsoft.Azure.Commands.ResourceManager.Automation.dll-Help.xml
online version: .\Get-AzureRmAutomationDscCompilationJob.md
schema: 2.0.0
ms.assetid: D1D461AB-138F-42F2-8FAF-E651A8310B08
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Automation/v1.0.12/Start-AzureRmAutomationDscCompilationJob.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Automation/v1.0.12/Start-AzureRmAutomationDscCompilationJob.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: 
keywords: powershell, cmdlet
---

# Start-AzureRmAutomationDscCompilationJob

## SYNOPSIS
Compiles a DSC configuration in Automation.

## SYNTAX

```
Start-AzureRmAutomationDscCompilationJob [-ConfigurationName] <String> [-Parameters <IDictionary>]
 [-ConfigurationData <IDictionary>] [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 [<CommonParameters>]
```

## DESCRIPTION
The **Start-AzureRmAutomationDscCompilationJob** cmdlet compiles an APS Desired State Configuration (DSC) configuration in azure_2 Automation.

## EXAMPLES

### Example 1: Compile an Azure DSC configuration in Automation
```
PS C:\>$Params = @{"StringParam"="Hello World";"IntegerParam"=32}
PS C:\> Start-AzureRmAutomationDscCompilationJob -ConfigurationName "Config01" -Parameters $Params -ResourceGroupName "ResourceGroup01"
```

The first command creates a dictionary of parameters, and stores them in the $Params variable.

The second command compiles the DSC configuration named Config01.
The command includes the values in $Params for DSC configuration parameters.

## PARAMETERS

### -AutomationAccountName
Specifies the name of the Automation account that contains the DSC configuration that this cmdlet compiles.

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

### -ConfigurationData
Specifies a dictionary of configuration data for DSC configuration.

```yaml
Type: IDictionary
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ConfigurationName
Specifies the name of the DSC configuration that this cmdlet compiles.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Name

Required: True
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Parameters
Specifies a dictionary of parameters that this cmdlet uses to compile the DSC configuration.

```yaml
Type: IDictionary
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of a resource group in which this cmdlet compiles a configuration.

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

## NOTES

## RELATED LINKS

[Get-AzureRmAutomationDscCompilationJob](xref:ResourceManager/AzureRM.Automation/v1.0.12/Get-AzureRmAutomationDscCompilationJob.md)

[Get-AzureRmAutomationDscCompilationJobOutput](xref:ResourceManager/AzureRM.Automation/v1.0.12/Get-AzureRmAutomationDscCompilationJobOutput.md)


