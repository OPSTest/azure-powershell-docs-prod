---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.Network.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 6AB403E4-ED81-4B11-8725-FCD441EB8CFD
updated_at: 11/1/2016 10:24 PM
ms.date: 11/1/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v3.0.0/Stop-AzureVirtualNetworkGatewayDiagnostics.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/f59f3ef60bc592383812213e69fd77ba950759ed/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v3.0.0/Stop-AzureVirtualNetworkGatewayDiagnostics.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: ServiceManagement_Azure_Networking_v3_0_0_Stop_AzureVirtualNetworkGatewayDiagnostics_md
---

# Stop-AzureVirtualNetworkGatewayDiagnostics

## SYNOPSIS
Stops a running virtual network gateway diagnostics session.

## SYNTAX

```
Stop-AzureVirtualNetworkGatewayDiagnostics [-GatewayId] <String> [-Profile <AzureSMProfile>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Stop-AzureVirtualNetworkGatewayDiagnostics** cmdlet stops a running virtual network gateway diagnostics session.
This command saves the results of the diagnostics session to the storage account that the Start-AzureVirtualNetworkGatewayDiagnostics cmdlet specifies.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -GatewayId
Specifies the ID of a gateway.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureVirtualNetworkGatewayDiagnostics](xref:ServiceManagement/Azure.Networking/v3.0.0/Get-AzureVirtualNetworkGatewayDiagnostics.md)

[Start-AzureVirtualNetworkGatewayDiagnostics](xref:ServiceManagement/Azure.Networking/v3.0.0/Start-AzureVirtualNetworkGatewayDiagnostics.md)


