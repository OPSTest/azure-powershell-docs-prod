---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 5698ECE0-59CD-4D84-855A-12886DF1E0C6
updated_at: 11/11/2016 11:03 PM
ms.date: 11/11/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.0.0/Resize-AzureRmVirtualNetworkGateway.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.0.0/Resize-AzureRmVirtualNetworkGateway.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/79eeb985ea480979357fb4695832a0c3d29a48bf/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.0.0/Resize-AzureRmVirtualNetworkGateway.md
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

# Resize-AzureRmVirtualNetworkGateway

## SYNOPSIS
Resizes an existing virtual network gateway.

## SYNTAX

```
Resize-AzureRmVirtualNetworkGateway -VirtualNetworkGateway <PSVirtualNetworkGateway> -GatewaySku <String>
 [<CommonParameters>]
```

## DESCRIPTION
The **Resize-AzureRmVirtualNetworkGateway** cmdlet enables you to change the stock-keeping unit (SKU) for a virtual network gateway.
SKUs determine the capabilities of a gateway, including such things as throughput and the maximum number of IP tunnels that are allowed.
Azure supports Basic, Standard, and High-Performance SKUs (sometimes referred to as Small, Medium, and Large SKUs).
For detailed information about the capabilities of each SKU type, see https://azure.microsoft.com/en-us/documentation/articles/vpn-gateway-about-vpngateways/.https://azure.microsoft.com/en-us/documentation/articles/vpn-gateway-about-vpngateways/.

Keep in mind that SKUs differ in pricing as well as capabilities.
For more information, see https://azure.microsoft.com/en-us/pricing/details/vpn-gateway/https://azure.microsoft.com/en-us/pricing/details/vpn-gateway/.

## EXAMPLES

### Example 1: Change the size of a virtual network gateway
```
PS C:\>$Gateway = Get-AzureRmVirtualNetworkGateway -Name "ContosoVirtualGateway"
PS C:\> Resize-AzureRmVirtualNetworkGateway -VirtualNetworkGateway $Gateway -GatewaySku "Basic"
```

This example changes the size of a virtual network gateway named ContosoVirtualGateway.

The first command creates an object reference to ContosoVirtualGateway; this object reference is stored in a variable named $Gateway.

The second command then uses the **Resize-AzureRmVirtualNetworkGateway** cmdlet to set the *GatewaySku* property to Basic.

## PARAMETERS

### -VirtualNetworkGateway
Specifies an object reference to the virtual network gateway to be resized.
You can create this object reference by using the Get-AzureRmVirtualNetworkGateway and specifying the name of the gateway.

```yaml
Type: PSVirtualNetworkGateway
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -GatewaySku
Specifies the new type of gateway SKU.
The acceptable values for this parameter are:

- Basic
- Standard
- High Performance

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

###  
This cmdlet accepts pipelined instances of the **Microsoft.Azure.Commands.Network.Models.PSVirtualNetworkGateway** object.

## OUTPUTS

###  
This cmdlet modifies existing instances of the **Microsoft.Azure.Commands.Network.Models.PSVirtualNetworkGateway** object.

## NOTES

## RELATED LINKS

[Get-AzureRmVpnClientPackage](xref:ResourceManager/AzureRM.Network/v3.0.0/Get-AzureRmVpnClientPackage.md)

[Get-AzureRmVirtualNetworkGateway](xref:ResourceManager/AzureRM.Network/v3.0.0/Get-AzureRmVirtualNetworkGateway.md)

[Set-AzureRmVirtualNetworkGatewayVpnClientConfig](xref:ResourceManager/AzureRM.Network/v3.0.0/Set-AzureRmVirtualNetworkGatewayVpnClientConfig.md)


