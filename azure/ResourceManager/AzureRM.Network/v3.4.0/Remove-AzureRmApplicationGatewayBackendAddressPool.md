---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
ms.assetid: F34C5D18-C505-4815-9DDB-C563E205515C
online version: 
schema: 2.0.0
updated_at: 1/20/2017 9:17 PM
ms.date: 1/20/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.4.0/Remove-AzureRmApplicationGatewayBackendAddressPool.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.4.0/Remove-AzureRmApplicationGatewayBackendAddressPool.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/cb06bb906911a2a2e1f57adbafe0c0c97a0b205b/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.4.0/Remove-AzureRmApplicationGatewayBackendAddressPool.md
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

# Remove-AzureRmApplicationGatewayBackendAddressPool

## SYNOPSIS
Removes a back-end address pool from an application gateway.

## SYNTAX

```
Remove-AzureRmApplicationGatewayBackendAddressPool -Name <String> -ApplicationGateway <PSApplicationGateway>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRmApplicationGatewayBackendAddressPool** cmdlet removes a back-end address pool from an Azure application gateway.

## EXAMPLES

### Example 1: Remove a back-end address pool from an application gateway
```
PS C:\>$AppGw = Get-AzureRmApplicationGateway -Name "ApplicationGateway01" -ResourceGroupName "ResourceGroup01"
PS C:\> Remove-AzureRmApplicationGatewayBackendAddressPool -ApplicationGateway $AppGw -Name "BackEndPool02"
```

The first command gets the application gateway named ApplicationGateway01 belonging to the resource group named ResourceGroup01 and saves it in the $AppGw variable.

The second command removes the back-end address pool named BackEndPool02 from the application gateway.

## PARAMETERS

### -ApplicationGateway
Specifies the application gateway from which this cmdlet removes a back-end address pool.

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
Specifies the name of the back-end address pool that this cmdlet removes.

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
Prompts you for confirmation before running the cmdlet.

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

### System.String

## OUTPUTS

## NOTES

## RELATED LINKS

[Add-AzureRmApplicationGatewayBackendAddressPool](xref:ResourceManager/AzureRM.Network/v3.4.0/Add-AzureRmApplicationGatewayBackendAddressPool.md)

[Get-AzureRmApplicationGatewayBackendAddressPool](xref:ResourceManager/AzureRM.Network/v3.4.0/Get-AzureRmApplicationGatewayBackendAddressPool.md)

[New-AzureRmApplicationGatewayBackendAddressPool](xref:ResourceManager/AzureRM.Network/v3.4.0/New-AzureRmApplicationGatewayBackendAddressPool.md)

[Set-AzureRmApplicationGatewayBackendAddressPool](xref:ResourceManager/AzureRM.Network/v3.4.0/Set-AzureRmApplicationGatewayBackendAddressPool.md)


