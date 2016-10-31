---
external help file: Microsoft.Azure.Commands.Automation.dll-Help.xml
online version: .\Get-AzureAutomationModule.md
schema: 2.0.0
ms.assetid: 24ACC1F1-F78A-4ECD-A996-31EC153F911C
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Automation/v0.9.8/Set-AzureAutomationModule.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.Automation/v0.9.8/Set-AzureAutomationModule.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Set-AzureAutomationModule

## SYNOPSIS
Updates a module in Azure Automation.

## SYNTAX

```
Set-AzureAutomationModule [-Name] <String> [-Tags <IDictionary>] [[-ContentLinkUri] <Uri>]
 [[-ContentLinkVersion] <String>] [-AutomationAccountName] <String> [-Profile <AzureProfile>]
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
Specifies the name of the automation account with the module.

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
Specifies the path to the module file.

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
Specifies the version of the module.

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

###  
Microsoft.Azure.Commands.Automation.Model.Module

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureAutomationModule](xref:ServiceManagement/Azure.Automation/v0.9.8/Get-AzureAutomationModule.md)

[New-AzureAutomationModule](xref:ServiceManagement/Azure.Automation/v0.9.8/New-AzureAutomationModule.md)

[Remove-AzureAutomationModule](xref:ServiceManagement/Azure.Automation/v0.9.8/Remove-AzureAutomationModule.md)


