---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: B7500E8A-578E-41A1-846A-06F93ECA26A4
updated_at: 11/11/2016 11:03 PM
ms.date: 11/11/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.0.0/New-AzureRmLoadBalancerBackendAddressPoolConfig.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.0.0/New-AzureRmLoadBalancerBackendAddressPoolConfig.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/79eeb985ea480979357fb4695832a0c3d29a48bf/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.0.0/New-AzureRmLoadBalancerBackendAddressPoolConfig.md
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

# New-AzureRmLoadBalancerBackendAddressPoolConfig

## SYNOPSIS
Creates a backend address pool configuration for a load balancer.

## SYNTAX

```
New-AzureRmLoadBalancerBackendAddressPoolConfig -Name <String> [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureRmLoadBalancerBackendAddressPoolConfig** cmdlet creates a backend address pool configuration for an Azure load balancer.

## EXAMPLES

### Example 1: Create a backend address pool configuration for a load balancer
```
PS C:\>New-AzureRmLoadBalancerBackendAddressPoolConfig -Name "BackendAddressPool02"
```

This command creates a backend address pool configuration named BackendAddressPool02 for a load balancer.

## PARAMETERS

### -Name
Specifies the name of the address pool configuration to create.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Add-AzureRmLoadBalancerBackendAddressPoolConfig](xref:ResourceManager/AzureRM.Network/v3.0.0/Add-AzureRmLoadBalancerBackendAddressPoolConfig.md)

[Get-AzureRmLoadBalancerBackendAddressPoolConfig](xref:ResourceManager/AzureRM.Network/v3.0.0/Get-AzureRmLoadBalancerBackendAddressPoolConfig.md)

[Remove-AzureRmLoadBalancerBackendAddressPoolConfig](xref:ResourceManager/AzureRM.Network/v3.0.0/Remove-AzureRmLoadBalancerBackendAddressPoolConfig.md)


