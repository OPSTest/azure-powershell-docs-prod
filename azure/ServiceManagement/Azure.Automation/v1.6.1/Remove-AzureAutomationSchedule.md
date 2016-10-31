---
external help file: Microsoft.Azure.Commands.Automation.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=397913
schema: 2.0.0
ms.assetid: DF785B56-2A2F-49AB-B23C-F06BD6B9FADE
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Automation/v1.6.1/Remove-AzureAutomationSchedule.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.Automation/v1.6.1/Remove-AzureAutomationSchedule.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Remove-AzureAutomationSchedule

## SYNOPSIS
Deletes an Azure Automation schedule.

## SYNTAX

```
Remove-AzureAutomationSchedule [-Name] <String> [-Force] [-AutomationAccountName] <String>
 [-Profile <AzureSMProfile>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureAutomationSchedule** cmdlet deletes a schedule from Microsoft Azure Automation.

## EXAMPLES

### Example 1: Remove a schedule
```
PS C:\> Remove-AzureAutomationSchedule -AutomationAccountName "Contoso17" -Name "MySchedule"
```

This command removes the schedule named MySchedule.

## PARAMETERS

### -AutomationAccountName
Specifies the name of an Automation account.

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

### -Force
Forces the command to run without asking for user confirmation.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the name of the schedule to remove.

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

### -Confirm
Prompts you for confirmation before running the cmdlet.Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Profile
In-memory profile.

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

[Get-AzureAutomationSchedule](xref:ServiceManagement/Azure.Automation/v1.6.1/Get-AzureAutomationSchedule.md)

[New-AzureAutomationSchedule](xref:ServiceManagement/Azure.Automation/v1.6.1/New-AzureAutomationSchedule.md)

[Set-AzureAutomationSchedule](xref:ServiceManagement/Azure.Automation/v1.6.1/Set-AzureAutomationSchedule.md)


