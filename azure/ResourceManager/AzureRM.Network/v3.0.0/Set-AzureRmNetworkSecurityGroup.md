---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version: 395b7084-ab6b-4765-b55a-1260f9c9ab1b
schema: 2.0.0
ms.assetid: E0696C25-4A2A-4E51-8A38-C1ADFBEFBAC0
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.0.0/Set-AzureRmNetworkSecurityGroup.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.0.0/Set-AzureRmNetworkSecurityGroup.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: 
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Set-AzureRmNetworkSecurityGroup

## SYNOPSIS
Sets the goal state for a network security group.

## SYNTAX

```
Set-AzureRmNetworkSecurityGroup -NetworkSecurityGroup <PSNetworkSecurityGroup> [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureRmNetworkSecurityGroup** cmdlet sets the goal state for an Azure network security group.

## EXAMPLES

### Example 1: Set the goal state for a network security group
```
PS C:\>Get-AzureRmNetworkSecurityGroup -Name "Nsg1" -ResourceGroupName "Rg1" | Add-AzureRmNetworkSecurityRuleConfig -Name "Rdp-Rule" -Description "Allow RDP" -Access "Allow" -Protocol "Tcp" -Direction "Inbound" -Priority 100 -SourceAddressPrefix "Internet" -SourcePortRange "*" -DestinationAddressPrefix "*" -DestinationPortRange "3389" | Set-AzureRmNetworkSecurityGroup
```

This command gets the Azure network security group named Nsg1, and adds a network security rule named Rdp-Rule to allow Internet traffic on port 3389 to the retrieved network security group object using Add-AzureRmNetworkSecurityRuleConfig.
The command persists the modified Azure network security group using **Set-AzureRmNetworkSecurityGroup**.

## PARAMETERS

### -NetworkSecurityGroup
A network security group object representing the goal state to which the cmdlet sets the network security group.

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

[Get-AzureRmNetworkSecurityGroup](xref:ResourceManager/AzureRM.Network/v3.0.0/Get-AzureRmNetworkSecurityGroup.md)

[New-AzureRmNetworkSecurityGroup](xref:ResourceManager/AzureRM.Network/v3.0.0/New-AzureRmNetworkSecurityGroup.md)

[Remove-AzureRmNetworkSecurityGroup](xref:ResourceManager/AzureRM.Network/v3.0.0/Remove-AzureRmNetworkSecurityGroup.md)


