---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.Network.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 3DE861AD-5A86-4C36-911C-EB695DAC1CF2
updated_at: 11/1/2016 10:24 PM
ms.date: 11/1/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v1.6.1/Remove-AzureVNetGateway.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/f59f3ef60bc592383812213e69fd77ba950759ed/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v1.6.1/Remove-AzureVNetGateway.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: ServiceManagement_Azure_Networking_v1_6_1_Remove_AzureVNetGateway_md
---

# Remove-AzureVNetGateway

## SYNOPSIS
Deletes a VPN gateway.

## SYNTAX

```
Remove-AzureVNetGateway [-VNetName] <String> [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureVNetGateway** cmdlet deletes an existing virtual private network (VPN) gateway for a virtual network.

## EXAMPLES

### Example 1: Remove a virtual network gateway
```
PS C:\>Remove-AzureVNetGateway -VNetName "ContosoVN07"
```

This command removes the virtual network gateway from the virtual network named ContosoVN07.

## PARAMETERS

### -VNetName
Specifies the virtual network in which this cmdlet deletes the VPN gateway.

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

[Get-AzureVNetGateway](xref:ServiceManagement/Azure.Networking/v1.6.1/Get-AzureVNetGateway.md)

[New-AzureVNetGateway](xref:ServiceManagement/Azure.Networking/v1.6.1/New-AzureVNetGateway.md)

[Reset-AzureVNetGateway](xref:ServiceManagement/Azure.Networking/v1.6.1/Reset-AzureVNetGateway.md)

[Resize-AzureVNetGateway](xref:ServiceManagement/Azure.Networking/v1.6.1/Resize-AzureVNetGateway.md)

[Set-AzureVNetGatewayKey](xref:ServiceManagement/Azure.Networking/v1.6.1/Set-AzureVNetGatewayKey.md)


