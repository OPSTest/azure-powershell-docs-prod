---
external help file: Microsoft.Azure.Commands.Automation.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 452BF685-28D4-4321-90FD-9C7FF4B2CF24
updated_at: 11/1/2016 10:24 PM
ms.date: 11/1/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ServiceManagement/Azure.Automation/v3.0.0/Remove-AzureAutomationCredential.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/f59f3ef60bc592383812213e69fd77ba950759ed/azureps-cmdlets-docs/ServiceManagement/Azure.Automation/v3.0.0/Remove-AzureAutomationCredential.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: ServiceManagement_Azure_Automation_v3_0_0_Remove_AzureAutomationCredential_md
---

# Remove-AzureAutomationCredential

## SYNOPSIS
Removes a credential from Automation.

## SYNTAX

```
Remove-AzureAutomationCredential [-Name] <String> [-Force] [-AutomationAccountName] <String>
 [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureAutomationCredential** cmdlet removes a credential from Microsoft Azure Automation.

## EXAMPLES

### Example 1: Remove a credential
```
PS C:\> Remove-AzureAutomationCredential -AutomationAccountName "Contoso17" -Name "MyCredential"
```

This command removes a credential named MyCredential in the Automation account named Contoso17.

## PARAMETERS

### -AutomationAccountName
Specifies the name of the Automation account with the credential.

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
Specifies the name of the credential to remove.

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

[Get-AzureAutomationCredential](xref:ServiceManagement/Azure.Automation/v3.0.0/Get-AzureAutomationCredential.md)

[New-AzureAutomationCredential](xref:ServiceManagement/Azure.Automation/v3.0.0/New-AzureAutomationCredential.md)

[Set-AzureAutomationCredential](xref:ServiceManagement/Azure.Automation/v3.0.0/Set-AzureAutomationCredential.md)


