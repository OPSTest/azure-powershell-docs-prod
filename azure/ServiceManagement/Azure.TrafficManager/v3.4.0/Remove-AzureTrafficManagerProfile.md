---
external help file: Microsoft.WindowsAzure.Commands.TrafficManager.dll-Help.xml
ms.assetid: B96A64DD-9005-4B04-A720-6FCF33797E8D
online version: 
schema: 2.0.0
updated_at: 1/20/2017 9:17 PM
ms.date: 1/20/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.TrafficManager/v3.4.0/Remove-AzureTrafficManagerProfile.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.TrafficManager/v3.4.0/Remove-AzureTrafficManagerProfile.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/cb06bb906911a2a2e1f57adbafe0c0c97a0b205b/azureps-cmdlets-docs/ServiceManagement/Azure.TrafficManager/v3.4.0/Remove-AzureTrafficManagerProfile.md
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

# Remove-AzureTrafficManagerProfile

## SYNOPSIS
Removes a Traffic Manager profile.

## SYNTAX

```
Remove-AzureTrafficManagerProfile [-Name] <String> [-Force] [-PassThru] [-Profile <AzureSMProfile>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureTrafficManagerProfile** cmdlet removes a Microsoft Azure Traffic Manager profile from the current subscription.

## EXAMPLES

### Example 1: Remove a Traffic Manager profile
```
PS C:\>Remove-AzureTrafficManagerProfile -Name "MyProfile"
```

This command removes the Traffic Manager profile named MyProfile.

### Example 2: Remove a Traffic Manager profile
```
PS C:\>Remove-AzureTrafficManagerProfile -Name "MyProfile" -Force -PassThru
```

This command removes the Traffic Manager profile named MyProfile without prompting you for confirmation, and returns the results.

## PARAMETERS

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
Specifies the name of the Traffic Manager profile to delete.

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

### -PassThru
Returns $True if the operation succeeded; otherwise, $False.
By default, this cmdlet does not generate any output.

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

### System.Boolean
This cmdlet generates $True or $False.
If the operation is successful and if you specify the *PassThru* parameter, this cmdlet returns a value of $True.

## NOTES

## RELATED LINKS

[Disable-AzureTrafficManagerProfile](xref:ServiceManagement/Azure.TrafficManager/v3.4.0/Disable-AzureTrafficManagerProfile.md)

[Enable-AzureTrafficManagerProfile](xref:ServiceManagement/Azure.TrafficManager/v3.4.0/Enable-AzureTrafficManagerProfile.md)

[Get-AzureTrafficManagerProfile](xref:ServiceManagement/Azure.TrafficManager/v3.4.0/Get-AzureTrafficManagerProfile.md)

[New-AzureTrafficManagerProfile](xref:ServiceManagement/Azure.TrafficManager/v3.4.0/New-AzureTrafficManagerProfile.md)

[Set-AzureTrafficManagerProfile](xref:ServiceManagement/Azure.TrafficManager/v3.4.0/Set-AzureTrafficManagerProfile.md)


