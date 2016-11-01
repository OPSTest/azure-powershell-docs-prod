---
external help file: Microsoft.WindowsAzure.Commands.RemoteApp.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 24893A50-F2FD-4B6A-81CC-B387B21105CD
updated_at: 11/1/2016 10:24 PM
ms.date: 11/1/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.RemoteApp/v1.6.1/Get-AzureRemoteAppVpnDeviceConfigScript.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/f59f3ef60bc592383812213e69fd77ba950759ed/azureps-cmdlets-docs/ServiceManagement/Azure.RemoteApp/v1.6.1/Get-AzureRemoteAppVpnDeviceConfigScript.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureRemoteAppVpnDeviceConfigScript

## SYNOPSIS
Retrieves the configuration script for an Azure RemoteApp VPN device.

## SYNTAX

```
Get-AzureRemoteAppVpnDeviceConfigScript [-VNetName] <String> [-Vendor] <String> [-Platform] <String>
 [-OSFamily] <String> [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRemoteAppVpnDeviceConfigScript** cmdlet retrieves the configuration script for an Azure RemoteApp virtual private network (VPN) device.

## EXAMPLES

### Example 1: Get a configuration script for a VPN device
```
PS C:\>Get-AzureRemoteAppVpnDeviceConfigScript -VNetName "ContosoVNet" -Vendor "Microsoft Corporation" -OSFamily "Windows Server 2012 R2"
```

This command returns the script or configuration file used to configure the VPN device for the virtual network named ContosoVNet.
This script or configuration file should be run or loaded onto the VPN device in the typical manner for that device.
Consult the VPN device vendor for the unique requirements for each device.

## PARAMETERS

### -OSFamily
Specifies the operating system (OS) family that runs on the device platform.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 4
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Platform
Specifies the device platform.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Vendor
Specifies the vendor of the VPN device.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -VNetName
Specifies the name of an Azure RemoteApp virtual network.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
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

[Get-AzureRemoteAppVpnDevice](xref:ServiceManagement/Azure.RemoteApp/v1.6.1/Get-AzureRemoteAppVpnDevice.md)


