---
external help file: Microsoft.WindowsAzure.Commands.RemoteApp.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 8576D0D9-588A-4E4F-9C94-31D140F34DDB
updated_at: 11/1/2016 10:24 PM
ms.date: 11/1/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.RemoteApp/v0.9.8/New-AzureRemoteAppVNet.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.RemoteApp/v0.9.8/New-AzureRemoteAppVNet.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/f59f3ef60bc592383812213e69fd77ba950759ed/azureps-cmdlets-docs/ServiceManagement/Azure.RemoteApp/v0.9.8/New-AzureRemoteAppVNet.md
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

# New-AzureRemoteAppVNet

## SYNOPSIS
Creates a RemoteApp virtual network.

## SYNTAX

```
New-AzureRemoteAppVNet -VNetName <String> -VirtualNetworkAddressSpace <String[]>
 -LocalNetworkAddressSpace <String[]> -DnsServerIpAddress <String[]> -VpnDeviceIpAddress <String>
 -Location <String> -GatewayType <GatewayType> [-Profile <AzureProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureRemoteAppVNet** cmdlet creates a Azure RemoteApp virtual network.

## EXAMPLES

### Example 1: Create a virtual network
```
PS C:\>New-AzureRemoteAppVnet -VNetName "ContosoVNet" -DnsServerIpAddress "192.168.0.5" -LocalNetworkAddressSpace "192.168.0.0/24" -Location "Central US" -VirtualNetworkAddressSpace "10.10.0.0/24" -VpnDeviceIpAddress "131.107.33.200" -GatewayType StaticRouting

TrackingId

----------

b0ca9d1b-d1b9-4f24-9a08-5e021926587f
```

This command creates a virtual network named ContosoVNet.

To determine the status of the operation, use the **Get-AzureRemoteAppOperationResult** cmdlet with the tracking ID that this cmdlet returns.

## PARAMETERS

### -DnsServerIpAddress
Specifies an array of the IPv4 addresses of the DNS servers.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -GatewayType
Specifies the type of gateway routing to use.
The acceptable values for this parameter are:  StaticRouting or DynamicRouting.

```yaml
Type: GatewayType
Parameter Sets: (All)
Aliases: 
Accepted values: StaticRouting, DynamicRouting

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -LocalNetworkAddressSpace
Specifies an array of strings that specify the local network address space, in Classless Interdomain Routing (CIDR) notation.
This address space must not overlap with the virtual network address space that the *VirtualNetworkAddressSpace* parameter specifies.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Location
Specifies the location in which to create the virtual network.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Profile
Specifies the Azure profile from which this cmdlet reads.
If you do not specify a profile, this cmdlet reads from the local default profile.

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

### -VNetName
Specifies the name of the Azure RemoteApp virtual network.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -VirtualNetworkAddressSpace
Specifies an array of string that specify the virtual network address space in CIDR notation.
This must be in the private IP address range and cannot overlap with the local network address space that the *LocalNetworkAddressSpace* parameter specifies.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -VpnDeviceIpAddress
Specifies the address of the virtual private network (VPN) device.
This must be a public-facing address.

```yaml
Type: String
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

[Get-AzureRemoteAppOperationResult](xref:ServiceManagement/Azure.RemoteApp/v0.9.8/Get-AzureRemoteAppOperationResult.md)

[Get-AzureRemoteAppVNet](xref:ServiceManagement/Azure.RemoteApp/v0.9.8/Get-AzureRemoteAppVNet.md)

[Remove-AzureRemoteAppVNet](xref:ServiceManagement/Azure.RemoteApp/v0.9.8/Remove-AzureRemoteAppVNet.md)

[Set-AzureRemoteAppVNet](xref:ServiceManagement/Azure.RemoteApp/v0.9.8/Set-AzureRemoteAppVNet.md)


