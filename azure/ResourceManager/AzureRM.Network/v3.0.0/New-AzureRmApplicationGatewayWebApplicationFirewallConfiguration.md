---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version: a34c2a52-6e9f-4878-a65c-7e6d1212c32f
schema: 2.0.0
ms.assetid: B1567E68-31EB-4C31-92E5-36A0487D118D
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.0.0/New-AzureRmApplicationGatewayWebApplicationFirewallConfiguration.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.0.0/New-AzureRmApplicationGatewayWebApplicationFirewallConfiguration.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: 
keywords: powershell, cmdlet
manager: visual-studio-china
---

# New-AzureRmApplicationGatewayWebApplicationFirewallConfiguration

## SYNOPSIS
Creates a WAF configuration for an application gateway.

## SYNTAX

```
New-AzureRmApplicationGatewayWebApplicationFirewallConfiguration -Enabled <Boolean> -FirewallMode <String>
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureRmApplicationGatewayWebApplicationFirewallConfiguration** cmdlet creates a web application firewall (WAF) configuration for an Azure application gateway.

## EXAMPLES

### Example 1: Create a web application firewall configuration for an application gateway
```
PS C:\>$FirewallConfig = New-AzureRmApplicationGatewayWebApplicationFirewallConfiguration -Enabled $True -FirewallMode "Prevention"
```

This command creates a configuiration that prevents requests when matched by the WAF, and then stores it in the $FirewallConfig variable.

## PARAMETERS

### -Enabled
Indicates whether the WAF is enabled.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -FirewallMode
Specifies the web application firewall mode.
The acceptable values for this parameter are:

- Detection
- Prevention

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

### -Confirm
Prompts you for confirmation before running the cmdlet.Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.Azure.Commands.Network.Models.PSApplicationGatewayWebApplicationFirewallConfiguration

## NOTES

## RELATED LINKS

[Get-AzureRmApplicationGatewayWebApplicationFirewallConfiguration](xref:ResourceManager/AzureRM.Network/v3.0.0/Get-AzureRmApplicationGatewayWebApplicationFirewallConfiguration.md)

[Set-AzureRmApplicationGatewayWebApplicationFirewallConfiguration](xref:ResourceManager/AzureRM.Network/v3.0.0/Set-AzureRmApplicationGatewayWebApplicationFirewallConfiguration.md)


