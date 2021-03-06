---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 862A9F99-999B-4178-BE74-B331CC674759
updated_at: 11/1/2016 10:24 PM
ms.date: 11/1/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v0.9.8/Set-AzureApplicationGatewayIPConfiguration.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v0.9.8/Set-AzureApplicationGatewayIPConfiguration.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/f59f3ef60bc592383812213e69fd77ba950759ed/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v0.9.8/Set-AzureApplicationGatewayIPConfiguration.md
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

# Set-AzureApplicationGatewayIPConfiguration

## SYNOPSIS
Modifies an IP configuration for an application gateway.

## SYNTAX

### SetByResourceId
```
Set-AzureApplicationGatewayIPConfiguration -ApplicationGateway <PSApplicationGateway> -Name <String>
 [-SubnetId <String>] [-Profile <AzureProfile>] [<CommonParameters>]
```

### SetByResource
```
Set-AzureApplicationGatewayIPConfiguration -ApplicationGateway <PSApplicationGateway> -Name <String>
 [-Subnet <PSSubnet>] [-Profile <AzureProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureApplicationGatewayIPConfiguration** cmdlet modifies an IP configuration.
An IP configuration contains the subnet in which an application gateway is deployed.

## EXAMPLES

### Example 1: Set the goal state of an IP configuration
```
PS C:\>$VNet = Get-AzureVirtualNetwork -Name "VNet01" -ResourceGroupName "ResourceGroup01"
PS C:\> $Subnet = Get-AzureVirtualNetworkSubnetConfig -Name "Subnet01" -VirtualNetwork $VNet 
PS C:\> $AppGw = Get-AzureApplicationGateway -Name "ApplicationGateway01" -ResourceGroupName "ResourceGroup01"
PS C:\> $AppGw = Set-AzureApplicationGatewayIPConfiguration -ApplicationGateway $AppGw 
-Name "AppgwSubnet01" -Subnet $Subnets
```

The first command gets the virtual network named VNet01 that belongs to the resource group named ResourceGroup01 and stores it in the $VNet variable.

The second command gets the subnet configuration named Subnet01 using $VNet and stores it in the $Subnet variable.

The third command gets an application gateway named ApplicationGateway01 that belongs to the resource group named ResourceGroup01 and stores it in the $AppGw variable.

The forth command sets the IP configuration of the application gateway stored in $AppGw to the subnet configuration stored in $Subnet.

## PARAMETERS

### -ApplicationGateway
Specifies an application gateway object with which this cmdlet associates an IP configuration.

```yaml
Type: PSApplicationGateway
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Name
Specifies the name of the IP configuration.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Profile
Specifies the Azure profile from which this cmdlet reads.
If you do not specify a profile, this cmdlet reads from the local default profile.

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

### -Subnet
Specifies the subnet.
This is the subnet in which the application gateway is deployed.

```yaml
Type: PSSubnet
Parameter Sets: SetByResource
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SubnetId
Specifies the subnet ID.
This is the subnet in which the application gateway is deployed.

```yaml
Type: String
Parameter Sets: SetByResourceId
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

### System.String

### Microsoft.Azure.Commands.Network.Models.PSSubnet

## OUTPUTS

### Microsoft.Azure.Commands.Network.Models.PSApplicationGateway

## NOTES

## RELATED LINKS

[Add-AzureApplicationGatewayIPConfiguration](xref:ResourceManager/AzureRM.Network/v0.9.8/Add-AzureApplicationGatewayIPConfiguration.md)

[Get-AzureApplicationGatewayIPConfiguration](xref:ResourceManager/AzureRM.Network/v0.9.8/Get-AzureApplicationGatewayIPConfiguration.md)

[New-AzureApplicationGatewayIPConfiguration](xref:ResourceManager/AzureRM.Network/v0.9.8/New-AzureApplicationGatewayIPConfiguration.md)

[Remove-AzureApplicationGatewayIPConfiguration](xref:ResourceManager/AzureRM.Network/v0.9.8/Remove-AzureApplicationGatewayIPConfiguration.md)


