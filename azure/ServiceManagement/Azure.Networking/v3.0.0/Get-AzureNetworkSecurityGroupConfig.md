---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.Network.dll-Help.xml
online version: 4b20f422-f5d6-403e-8744-2757c54ef0d4
schema: 2.0.0
ms.assetid: 04829021-EF5F-48A7-888D-8C14ADFFAC8C
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v3.0.0/Get-AzureNetworkSecurityGroupConfig.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v3.0.0/Get-AzureNetworkSecurityGroupConfig.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: PowerShellHelpPub
---

# Get-AzureNetworkSecurityGroupConfig

## SYNOPSIS
Gets details for a network security group.

## SYNTAX

```
Get-AzureNetworkSecurityGroupConfig [-Detailed] -VM <IPersistentVM> [-Profile <AzureSMProfile>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureNetworkSecurityGroupConfig** cmdlet returns details for a network security group.
Specify the *Detailed* parameter to display the network security rules.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -Detailed
Indicates that this cmdlet displays the network security rules.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
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

### -VM
Specifies the virtual machine for which this cmdlet gets the details of a network security group.

```yaml
Type: IPersistentVM
Parameter Sets: (All)
Aliases: InputObject

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[New-AzureNetworkSecurityGroup](./New-AzureNetworkSecurityGroup.md)

[Remove-AzureNetworkSecurityGroup](./Remove-AzureNetworkSecurityGroup.md)


