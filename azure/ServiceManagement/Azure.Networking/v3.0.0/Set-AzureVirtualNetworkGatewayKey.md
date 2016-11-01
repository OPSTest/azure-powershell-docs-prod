---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.Network.dll-Help.xml
online version: 48b9d59d-ff51-4f70-9a29-fd017a9a8383
schema: 2.0.0
ms.assetid: 55E48183-31B6-44C7-A94B-E75D28415585
updated_at: 11/1/2016 8:11 PM
ms.date: 11/1/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v3.0.0/Set-AzureVirtualNetworkGatewayKey.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/76d389e6f4656b8cb2f1cc90ba2be7be7f3ff754/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v3.0.0/Set-AzureVirtualNetworkGatewayKey.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Set-AzureVirtualNetworkGatewayKey

## SYNOPSIS
Sets the key for an Azure virtual network gateway.

## SYNTAX

```
Set-AzureVirtualNetworkGatewayKey [-GatewayId] <String> [-ConnectedEntityId] <String> [-SharedKey] <String>
 [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureVirtualNetworkGatewayKey** cmdlet sets the key for an Azure virtual network gateway.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -ConnectedEntityId
Specifies the ID of a connected entity.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -GatewayId
Specifies the ID of a gateway

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
Specifies the Azure profile from which this cmdlet reads. 
If you do not specify a profile, this cmdlet reads from the local default profile.
By default, this cmdlet does not generate any output.

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

### -SharedKey
Specifies a shared key.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
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

[Get-AzureVirtualNetworkGatewayKey](xref:ServiceManagement/Azure.Networking/v3.0.0/Get-AzureVirtualNetworkGatewayKey.md)

[Reset-AzureVirtualNetworkGatewayKey](xref:ServiceManagement/Azure.Networking/v3.0.0/Reset-AzureVirtualNetworkGatewayKey.md)


