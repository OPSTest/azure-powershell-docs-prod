---
external help file: Microsoft.WindowsAzure.Commands.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 6293F1AE-4E8A-4462-9038-30E5B7787359
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v3.0.0/New-WAPackStaticIPAddressPool.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v3.0.0/New-WAPackStaticIPAddressPool.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: 
keywords: powershell, cmdlet
manager: visual-studio-china
---

# New-WAPackStaticIPAddressPool

## SYNOPSIS
Creates a static IP address pool.

## SYNTAX

```
New-WAPackStaticIPAddressPool -VMSubnet <VMSubnet> -Name <String> -IPAddressRangeStart <String>
 -IPAddressRangeEnd <String> [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
These topics are deprecated and will be removed in the future.
For the updated topics, see  Azure WAPack Cmdletshttp://msdn.microsoft.com/library/dn776450.aspx.
This topic describes the cmdlet in the 0.8.1 version of the Microsoft Azure PowerShell module.
To find out the version of the module you're using, from the Azure PowerShell console, type (get-module azure).version.

The **New-WAPackStaticIPAddressPool** cmdlet creates a static IP address pool.

## EXAMPLES

### Example 1: Create a static IP address pool
```
PS C:\>$VNet = Get-WAPackVNet -Name "ContosoVNet01"
PS C:\>$VMSubnet = Get-WAPackVMSubnet ?VNet $VNet -Name "ContosoVMSubnet01"
PS C:\>New-WAPackStaticIpAddressPool ?VMSubnet $VMSubnet -Name "ContosoStaticIpAddressPool01" -IPAddressRangeStart "192.168.1.0" -IPAddressRangeEnd "192.168.1.10"
```

The first command first retrieves the virtual machine network to which we want to add the static IP address pool.
This virtual machine network is named ContosoVNet01.
The second command uses the previously retrieved virtual machine network to get the virtual machine subnet named ContosoVMSubnet01 to which we want to add the static IP address pool.
The third and last command creates a new static IP address pool with a name ContosoStaticIpAddressPool01 and a range start 192.168.1.0 and a range end 192.168.1.10.

## PARAMETERS

### -VMSubnet
Specifies a VMSubnet associated with the static IP address pool.

```yaml
Type: VMSubnet
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Name
Specifies a name for the static IP address pool.

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

### -IPAddressRangeStart
Specifies an IP address range start for the static IP address pool.

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

### -IPAddressRangeEnd
Specifies an IP address range end for the static IP address pool.

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

[Get-WAPackStaticIPAddressPool](./Get-WAPackStaticIPAddressPool.md)

[Remove-WAPackStaticIPAddressPool](./Remove-WAPackStaticIPAddressPool.md)


