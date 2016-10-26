---
external help file: Microsoft.Azure.Commands.Automation.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=397916
schema: 2.0.0
ms.assetid: 595C26F0-6401-43D4-A70C-491FB2EF2696
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Automation/v0.9.8/Set-AzureAutomationRunbookDefinition.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.Automation/v0.9.8/Set-AzureAutomationRunbookDefinition.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: 
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Set-AzureAutomationRunbookDefinition

## SYNOPSIS
Updates the draft definition of a runbook.

## SYNTAX

```
Set-AzureAutomationRunbookDefinition [-Name] <String> [-Path] <String> [-Overwrite]
 [-AutomationAccountName] <String> [-Profile <AzureProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureAutomationRunbookDefinition** cmdlet updates the draft definition of a Microsoft Azure Automation runbook.
Provide a Windows PowerShell ‚Â® script (.ps1) file that contains a runbook which becomes the draft runbook.
If a draft already exists, use the *Overwrite* parameter to force the cmdlet to overwrite the existing draft.

## EXAMPLES

### Example 1: Overwrite an existing draft definition of a runbook
```
PS C:\> Set-AzureAutomationRunbookDefinition -AutomationAccountName "Contoso17" -Name "Runbk01" -Path .\App01.ps1 -Overwrite
```

This command overwrites the existing draft definition of a runbook.

## PARAMETERS

### -AutomationAccountName
@{Text=}

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
@{Text=}

```yaml
Type: String
Parameter Sets: (All)
Aliases: RunbookName

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Overwrite
@{Text=}

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

### -Path
@{Text=}

```yaml
Type: String
Parameter Sets: (All)
Aliases: RunbookPath

Required: True
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Profile
In-memory profile.

```yaml
Type: AzureProfile
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

### Microsoft.Azure.Commands.Automation.Model.RunbookDefinition

## NOTES

## RELATED LINKS

[Get-AzureAutomationRunbookDefinition](./Get-AzureAutomationRunbookDefinition.md)


