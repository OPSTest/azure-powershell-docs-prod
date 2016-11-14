---
external help file: Microsoft.Azure.Commands.Automation.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 73EC65F6-7716-4040-8DA0-86EFA9D2FDF2
updated_at: 11/11/2016 11:03 PM
ms.date: 11/11/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ServiceManagement/Azure.Automation/v2.1.0/Set-AzureAutomationModule.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/79eeb985ea480979357fb4695832a0c3d29a48bf/azureps-cmdlets-docs/ServiceManagement/Azure.Automation/v2.1.0/Set-AzureAutomationModule.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: ServiceManagement_Azure_Automation_v2_1_0_Set_AzureAutomationModule_md
---

# Set-AzureAutomationModule

## SYNOPSIS
Updates a module in Automation.

## SYNTAX

```
Set-AzureAutomationModule [-Name] <String> [-Tags <IDictionary>] [[-ContentLinkUri] <Uri>]
 [[-ContentLinkVersion] <String>] [-AutomationAccountName] <String> [-Profile <AzureSMProfile>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureAutomationModule** cmdlet imports a new version of a module or changes the configuration of the module in Azure Automation.

## EXAMPLES

### Example 1: Update a module
```
PS C:\> Set-AzureAutomationModule  ¢â‚¬"AutomationAccountName "Contoso17"  ¢â‚¬"Name "ContosoModule"  ¢â‚¬"ContentLinkUri ".\ContosoModule.zip"  ¢â‚¬"ContentLinkVersion "1.1"
```

This command imports an updated version of an existing module named ContosoModule into the Azure Automation account named Contoso17.

## PARAMETERS

### -AutomationAccountName

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

### -ContentLinkUri

```yaml
Type: Uri
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ContentLinkVersion

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name

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

### -Tags

```yaml
Type: IDictionary
Parameter Sets: (All)
Aliases: Tag

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Profile

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

### Microsoft.Azure.Commands.Automation.Model.Module

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureAutomationModule](xref:ServiceManagement/Azure.Automation/v2.1.0/Get-AzureAutomationModule.md)

[New-AzureAutomationModule](xref:ServiceManagement/Azure.Automation/v2.1.0/New-AzureAutomationModule.md)

[Remove-AzureAutomationModule](xref:ServiceManagement/Azure.Automation/v2.1.0/Remove-AzureAutomationModule.md)


