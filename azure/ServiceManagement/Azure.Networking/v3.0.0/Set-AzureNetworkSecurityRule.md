---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.Network.dll-Help.xml
online version: 3cb862d2-c316-4135-a59a-65441f00ad96
schema: 2.0.0
ms.assetid: 045041BF-855D-47A2-9D18-9D4BBB0525EA
updated_at: 11/1/2016 8:11 PM
ms.date: 11/1/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v3.0.0/Set-AzureNetworkSecurityRule.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/76d389e6f4656b8cb2f1cc90ba2be7be7f3ff754/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v3.0.0/Set-AzureNetworkSecurityRule.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Set-AzureNetworkSecurityRule

## SYNOPSIS
Adds or modifies a network security rule in a network security group.

## SYNTAX

```
Set-AzureNetworkSecurityRule -Name <String> -Type <String> -Priority <Int32> -Action <String>
 -SourceAddressPrefix <String> -SourcePortRange <String> -DestinationAddressPrefix <String>
 -DestinationPortRange <String> -Protocol <String> [-NetworkSecurityGroup] <INetworkSecurityGroup>
 [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureNetworkSecurityRule** cmdlet adds or modifies an Azure network security rule in a network security group.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -Name
Specifies the name for the network security rule that this cmdlet adds or modifies.

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

### -Type
Specifies the type of connection for the network security rule.
Valid values are: Inbound and Outbound.

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

### -Priority
Specifies the priority for the network security rule.
Valid values are: integers from 100 to 4096.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Action
Specifies the action for a network security rule.
Valid values are: Allow and Deny.

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

### -SourceAddressPrefix
Specifies the CIDR address of the source IP range for the network security rule.
An asterisk (*) specifies any IP address.

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

### -SourcePortRange
Specifies a source port range for the network security rule.
Valid values consist of integers from 0 to 65535.
You can specify an individual value, or specify a range in the format LowerNumber-HigherNumber.
A hyphen separates the two values.

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

### -DestinationAddressPrefix
Specifies the Classless Interdomain Routing (CIDR) address of the destination IP range for the network security rule.
An asterisk (*) specifies any IP address.

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

### -DestinationPortRange
Specifies a destination port range for the network security rule.
Valid values consist of integers from 0 to 65535.
You can specify an individual value, or specify a range in the format LowerNumber-HigherNumber.
A hyphen separates the two values.

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

### -Protocol
Specifies the protocol for the network security rule.
Valid values are: 

- TCP 
- UDP 
- *

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

### -NetworkSecurityGroup
Specifies the network security group that this cmdlet modifies.
To obtain an **INetworkSecurityGroup** object, use the Get-AzureNetworkSecurityGroup cmdlet.

```yaml
Type: INetworkSecurityGroup
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
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

[Remove-AzureNetworkSecurityRule](xref:ServiceManagement/Azure.Networking/v3.0.0/Remove-AzureNetworkSecurityRule.md)


