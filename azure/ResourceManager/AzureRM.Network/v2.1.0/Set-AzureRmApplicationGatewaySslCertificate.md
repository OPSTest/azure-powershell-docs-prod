---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version: .\Add-AzureRmApplicationGatewaySslCertificate.md
schema: 2.0.0
ms.assetid: 3014BB49-395A-4C4E-A3AA-8048EF9E5701
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v2.1.0/Set-AzureRmApplicationGatewaySslCertificate.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v2.1.0/Set-AzureRmApplicationGatewaySslCertificate.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Set-AzureRmApplicationGatewaySslCertificate

## SYNOPSIS
Sets the goal state of an SSL certificate.

## SYNTAX

```
Set-AzureRmApplicationGatewaySslCertificate -ApplicationGateway <PSApplicationGateway> -Name <String>
 -CertificateFile <String> -Password <String> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureRmApplicationGatewaySslCertificate** cmdlet sets the goal state of an SSL certificate.

## EXAMPLES

### Example 1: Set the goal state of an SSL certificate
```
PS C:\>$AppGW = Get-AzureRmApplicationGateway -Name "ApplicationGateway01" -ResourceGroupName "ResourceGroup01"
PS C:\> $Cert = Set-AzureRmApplicationGatewaySslCertificate -ApplicationGateway $AppGW -Name "Cert01" -CertificateFile "D:\cert01.pfx" -Password "Password01"
```

This command sets the goal state for an SSL certificate from the application gateway named ApplicationGateway01.

## PARAMETERS

### -ApplicationGateway
Specifies the application gateway with which the Secure Socket Layer (SSL) certificate is associated.

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
Specifies the name of the SSL certificate.

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

### -CertificateFile
Specifies the path of the SSL certificate.

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

### -Password
Specifies the password of the SSL certificate.

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

### Microsoft.Azure.Commands.Network.Models.PSApplicationGateway

## NOTES

## RELATED LINKS

[Add-AzureRmApplicationGatewaySslCertificate](xref:ResourceManager/AzureRM.Network/v2.1.0/Add-AzureRmApplicationGatewaySslCertificate.md)

[Get-AzureRmApplicationGatewaySslCertificate](xref:ResourceManager/AzureRM.Network/v2.1.0/Get-AzureRmApplicationGatewaySslCertificate.md)

[New-AzureRmApplicationGatewaySslCertificate](xref:ResourceManager/AzureRM.Network/v2.1.0/New-AzureRmApplicationGatewaySslCertificate.md)

[Remove-AzureRmApplicationGatewaySslCertificate](xref:ResourceManager/AzureRM.Network/v2.1.0/Remove-AzureRmApplicationGatewaySslCertificate.md)


