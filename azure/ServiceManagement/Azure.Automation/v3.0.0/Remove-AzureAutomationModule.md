---
external help file: Microsoft.Azure.Commands.Automation.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 75C8C7A7-FCE8-4E3C-8469-2A0773B63C38
updated_at: 11/11/2016 11:03 PM
ms.date: 11/11/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ServiceManagement/Azure.Automation/v3.0.0/Remove-AzureAutomationModule.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/79eeb985ea480979357fb4695832a0c3d29a48bf/azureps-cmdlets-docs/ServiceManagement/Azure.Automation/v3.0.0/Remove-AzureAutomationModule.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: ServiceManagement_Azure_Automation_v3_0_0_Remove_AzureAutomationModule_md
---

# Remove-AzureAutomationModule

## SYNOPSIS
Removes a module from Automation.

## SYNTAX

```
Remove-AzureAutomationModule [-Name] <String> [-Force] [-AutomationAccountName] <String>
 [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureAutomationModule** cmdlet removes an Automation account from Microsoft Azure Automation.

## EXAMPLES

### Example 1: Remove a module
```
PS C:\> Remove-AzureAutomationModule  ¢â‚¬"AutomationAccountName "Contoso17"  ¢â‚¬"Name "ContosoModule"
```

This command removes a module named ContosoModule from the Automation account named Contoso17.

## PARAMETERS

### -AutomationAccountName
Specifies the name of the Automation account with the module.

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
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the name of the module to remove.

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

[Get-AzureAutomationModule](xref:ServiceManagement/Azure.Automation/v3.0.0/Get-AzureAutomationModule.md)

[New-AzureAutomationModule](xref:ServiceManagement/Azure.Automation/v3.0.0/New-AzureAutomationModule.md)

[Set-AzureAutomationModule](xref:ServiceManagement/Azure.Automation/v3.0.0/Set-AzureAutomationModule.md)


