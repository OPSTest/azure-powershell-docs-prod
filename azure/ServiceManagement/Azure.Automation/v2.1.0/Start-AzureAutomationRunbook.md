---
external help file: Microsoft.Azure.Commands.Automation.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=397918
schema: 2.0.0
ms.assetid: 1A7B620D-2C3F-4A47-9E61-860164A70F43
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Automation/v2.1.0/Start-AzureAutomationRunbook.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.Automation/v2.1.0/Start-AzureAutomationRunbook.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Start-AzureAutomationRunbook

## SYNOPSIS
Starts a runbook job.

## SYNTAX

```
Start-AzureAutomationRunbook -Name <String> [-Parameters <IDictionary>] [-RunOn <String>]
 [-AutomationAccountName] <String> [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Start-AzureAutomationRunbook** cmdlet starts a Microsoft Azure Automation runbook job.
Specify the ID or name of a runbook.

## EXAMPLES

### Example 1: Start a runbook job
```
PS C:\> Start-AzureAutomationRunbook -AutomationAccountName "Contoso17" -Name "Runbk01"
```

This command starts a runbook job for the runbook named Runbk01 in the Automation account named Contoso17.

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

### -Name
Specifies the name of a runbook.

```yaml
Type: String
Parameter Sets: (All)
Aliases: RunbookName

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Parameters
@{Text=}

```yaml
Type: IDictionary
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Profile
@{Text=}

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

### -RunOn
@{Text=}

```yaml
Type: String
Parameter Sets: (All)
Aliases: HybridWorker

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

### Microsoft.Azure.Commands.Automation.Model.Job

## NOTES

## RELATED LINKS

[Get-AzureAutomationRunbook](xref:ServiceManagement/Azure.Automation/v2.1.0/Get-AzureAutomationRunbook.md)

[New-AzureAutomationRunbook](xref:ServiceManagement/Azure.Automation/v2.1.0/New-AzureAutomationRunbook.md)

[Publish-AzureAutomationRunbook](xref:ServiceManagement/Azure.Automation/v2.1.0/Publish-AzureAutomationRunbook.md)

[Remove-AzureAutomationRunbook](xref:ServiceManagement/Azure.Automation/v2.1.0/Remove-AzureAutomationRunbook.md)

[Set-AzureAutomationRunbook](xref:ServiceManagement/Azure.Automation/v2.1.0/Set-AzureAutomationRunbook.md)


