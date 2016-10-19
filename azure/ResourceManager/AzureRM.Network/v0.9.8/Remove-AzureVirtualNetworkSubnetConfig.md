---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version: .\Add-AzureVirtualNetworkSubnetConfig.md
schema: 2.0.0
ms.assetid: 7EDD7D1F-65A8-4AB5-A713-3E8A3D1ADCE8
updated_at: 10/18/2016 9:38 PM
ms.date: 10/18/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v0.9.8/Remove-AzureVirtualNetworkSubnetConfig.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/23cdb8705d4ab9807c0e21b238f3b134a7d49c7d/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v0.9.8/Remove-AzureVirtualNetworkSubnetConfig.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Remove-AzureVirtualNetworkSubnetConfig

## SYNOPSIS
Removes a subnet configuration from a virtual network.

## SYNTAX

```
Remove-AzureVirtualNetworkSubnetConfig [-Name <String>] -VirtualNetwork <PSVirtualNetwork>
 [-Profile <AzureProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureVirtualNetworkSubnetConfig** cmdlet removes a subnet from an Azure virtual network.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -Name
Specifies the name of the subnet configuration to remove.

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

### -Profile
Specifies an Azure profile.

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

### -VirtualNetwork
Specifies the **VirtualNetwork** object that contains the subnet configuration to remove.

```yaml
Type: PSVirtualNetwork
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

[Add-AzureVirtualNetworkSubnetConfig](.\Add-AzureVirtualNetworkSubnetConfig.md)

[Get-AzureVirtualNetworkSubnetConfig](.\Get-AzureVirtualNetworkSubnetConfig.md)

[New-AzureVirtualNetworkSubnetConfig](.\New-AzureVirtualNetworkSubnetConfig.md)

[Set-AzureVirtualNetworkSubnetConfig](.\Set-AzureVirtualNetworkSubnetConfig.md)

