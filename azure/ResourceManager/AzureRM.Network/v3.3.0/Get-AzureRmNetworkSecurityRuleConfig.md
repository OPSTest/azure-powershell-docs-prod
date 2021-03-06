---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
ms.assetid: 5A0D9326-3A8A-4156-8372-EBA93C1BB4E4
online version: 
schema: 2.0.0
updated_at: 1/27/2017 5:12 PM
ms.date: 1/27/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.3.0/Get-AzureRmNetworkSecurityRuleConfig.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.3.0/Get-AzureRmNetworkSecurityRuleConfig.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/84ef3e6f08e94eaea317c9834c9680310d7de7c4/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.3.0/Get-AzureRmNetworkSecurityRuleConfig.md
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

# Get-AzureRmNetworkSecurityRuleConfig

## SYNOPSIS
Get a network security rule configuration for a network security group.

## SYNTAX

```
Get-AzureRmNetworkSecurityRuleConfig [-Name <String>] -NetworkSecurityGroup <PSNetworkSecurityGroup>
 [-DefaultRules] [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmNetworkSecurityRuleConfig** cmdlet gets a network security rule configuration for an Azure network security group.

## EXAMPLES

### Example 1: Get a network security rule configuration
```
PS C:\> Get-AzureRmNetworkSecurityGroup -Name  "NSG01" -ResourceGroupName "ResourceGroup03" | Get-AzureRmNetworkSecurityRuleConfig -Name "AllowInternetOutBound" -DefaultRules
```

This command gets a network security group named NSG01 in ResourceGroup03, and then passes it to the current cmdlet. 
The command retrieves the default rule named AllowInternetOutBound from that group.

### Example 2: Retrieving a network security rule config using only the name
```
PS C:\> Get-AzureRmNetworkSecurityGroup -Name  "NSG01" -ResourceGroupName ResourceGroup03 | Get-AzureRmNetworkSecurityRuleConfig -Name "rdp-rule"
```

This command gets a network security group named NSG01 in ResourceGroup03, and then passes it to the current cmdlet. 
The command retrieves user defined rule named rdp-rule from that group.

## PARAMETERS

### -DefaultRules
Indicates whether this cmdlet gets a user-created rule configuration or a default rule configuration.

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

### -InformationAction
Specifies how this cmdlet responds to an information event.

The acceptable values for this parameter are:

- Continue
- Ignore
- Inquire
- SilentlyContinue
- Stop
- Suspend

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
Specifies an information variable.

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the name of the network security rule configuration to get.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NetworkSecurityGroup
Specifies a **NetworkSecurityGroup** object that contains the network security rule configuration to get.

```yaml
Type: PSNetworkSecurityGroup
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Add-AzureRmNetworkSecurityRuleConfig](xref:ResourceManager/AzureRM.Network/v3.3.0/Add-AzureRmNetworkSecurityRuleConfig.md)

[Get-AzureRmNetworkSecurityGroup](xref:ResourceManager/AzureRM.Network/v3.3.0/Get-AzureRmNetworkSecurityGroup.md)

[New-AzureRmNetworkSecurityRuleConfig](xref:ResourceManager/AzureRM.Network/v3.3.0/New-AzureRmNetworkSecurityRuleConfig.md)

[Remove-AzureRmNetworkSecurityRuleConfig](xref:ResourceManager/AzureRM.Network/v3.3.0/Remove-AzureRmNetworkSecurityRuleConfig.md)

[Set-AzureRmNetworkSecurityRuleConfig](xref:ResourceManager/AzureRM.Network/v3.3.0/Set-AzureRmNetworkSecurityRuleConfig.md)


