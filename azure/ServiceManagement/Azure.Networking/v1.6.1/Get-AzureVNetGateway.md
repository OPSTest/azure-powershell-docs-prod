---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.Network.dll-Help.xml
online version: .\New-AzureVNetGateway.md
schema: 2.0.0
ms.assetid: 12E991FE-45C2-48C6-AF0F-738D93021E5C
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v1.6.1/Get-AzureVNetGateway.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v1.6.1/Get-AzureVNetGateway.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureVNetGateway

## SYNOPSIS
Gets the status of a virtual network gateway.

## SYNTAX

```
Get-AzureVNetGateway [-VNetName] <String> [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureVNetGateway** cmdlet gets the status of an existing virtual network gateway.

## EXAMPLES

### Example 1: Get the status of a virtual network gateway
```
PS C:\>Get-AzureVNetGateway -VNetName "ContosoVN07"
```

This command gets that status of the virtual network gateway for the virtual network named ContosoVN07.

## PARAMETERS

### -VNetName
Specifies the virtual network that contains the virtual network gateway for which this cmdlet gets status.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Profile
ps_azureprofile_description

```yaml
Type: AzureSMProfile
Parameter Sets: (All)
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

## OUTPUTS

## NOTES

## RELATED LINKS

[New-AzureVNetGateway](xref:ServiceManagement/Azure.Networking/v1.6.1/New-AzureVNetGateway.md)

[Remove-AzureVNetGateway](xref:ServiceManagement/Azure.Networking/v1.6.1/Remove-AzureVNetGateway.md)

[Reset-AzureVNetGateway](xref:ServiceManagement/Azure.Networking/v1.6.1/Reset-AzureVNetGateway.md)

[Resize-AzureVNetGateway](xref:ServiceManagement/Azure.Networking/v1.6.1/Resize-AzureVNetGateway.md)

[Set-AzureVNetGatewayKey](xref:ServiceManagement/Azure.Networking/v1.6.1/Set-AzureVNetGatewayKey.md)


