---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version: .\Add-AzureRmApplicationGatewayFrontendIPConfig.md
schema: 2.0.0
ms.assetid: C9975C73-AA56-4BE4-8DE0-2F63597AB52E
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v1.0.13/Remove-AzureRmApplicationGatewayFrontendIPConfig.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v1.0.13/Remove-AzureRmApplicationGatewayFrontendIPConfig.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Remove-AzureRmApplicationGatewayFrontendIPConfig

## SYNOPSIS
Removes a front-end IP configuration from an application gateway.

## SYNTAX

```
Remove-AzureRmApplicationGatewayFrontendIPConfig -Name <String> -ApplicationGateway <PSApplicationGateway>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRmApplicationGatewayFrontendIPConfig** cmdlet removes frontend IP from an azure_2 application gateway.

## EXAMPLES

### Example 1: Remove a front-end IP configuration
```
PS C:\>$AppGw = Get-AzureRmApplicationGateway -Name "ApplicationGateway01" -ResourceGroupName "ResourceGroup01"
PS C:\> Remove-AzureRmApplicationGatewayFrontendIPConfig -ApplicationGateway $AppGw -Name "FrontEndIP02"
```

The first command gets an application gateway named ApplicationGateway01 and stores it in the $AppGw variable.

The second command removes the front-end IP configuration named FrontEndIP02 from the application gateway stored in $AppGw.

## PARAMETERS

### -Name
Specifies the name of a front-end IP configuration to remove.

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

### -ApplicationGateway
Specifies an application gateway from which to remove a front-end IP configuration.

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
@{Text=}

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
@{Text=}

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String

## OUTPUTS

## NOTES

## RELATED LINKS

[Add-AzureRmApplicationGatewayFrontendIPConfig](xref:ResourceManager/AzureRM.Network/v1.0.13/Add-AzureRmApplicationGatewayFrontendIPConfig.md)

[Get-AzureRmApplicationGatewayFrontendIPConfig](xref:ResourceManager/AzureRM.Network/v1.0.13/Get-AzureRmApplicationGatewayFrontendIPConfig.md)

[New-AzureRmApplicationGatewayFrontendIPConfig](xref:ResourceManager/AzureRM.Network/v1.0.13/New-AzureRmApplicationGatewayFrontendIPConfig.md)

[Set-AzureRmApplicationGatewayFrontendIPConfig](xref:ResourceManager/AzureRM.Network/v1.0.13/Set-AzureRmApplicationGatewayFrontendIPConfig.md)


