---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
ms.assetid: F253FB21-37EF-41C9-A079-908DE3BB5AFA
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.1.0/Get-AzureRmVirtualNetworkPeering.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.1.0/Get-AzureRmVirtualNetworkPeering.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: ResourceManager_AzureRM_Network_v3_1_0_Get_AzureRmVirtualNetworkPeering_md
---

# Get-AzureRmVirtualNetworkPeering

## SYNOPSIS
Gets the virtual network peering.

## SYNTAX

```
Get-AzureRmVirtualNetworkPeering -VirtualNetworkName <String> -ResourceGroupName <String> [-Name <String>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmVirtualNetworkPeering** cmdlet gets the virtual network peering.

## EXAMPLES

### Example 1: Get a peering between two virtual networks
```
PS C:\>Get-AzureRmVirtualNetworkPeering -Name "LinkToVNet2" -VirtualNetwork "MyVirtualNetwork" -ResourceGroupName "MyResourceGroup"
```

This command gets a previously created virtual network peering named LinkToVNet2 located in MyVirtualNetwork in the resource group named MyResourceGroup.

## PARAMETERS

### -VirtualNetworkName
Specifies the virtual network name that this cmdlet gets.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the resource group name that the virtual network peering belongs to.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the virtual network peering name.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -InformationAction
Specifies how this cmdlet responds to an information event.

The acceptable values for this parameter are:

- Continue
- Ignore
- Inquire
- SilentlyContinue
- Stop
- Suspend

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
Specifies an information variable.

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

## OUTPUTS

## NOTES

## RELATED LINKS

[Add-AzureRmVirtualNetworkPeering](xref:ResourceManager/AzureRM.Network/v3.1.0/Add-AzureRmVirtualNetworkPeering.md)

[Remove-AzureRmVirtualNetworkPeering](xref:ResourceManager/AzureRM.Network/v3.1.0/Remove-AzureRmVirtualNetworkPeering.md)

[Set-AzureRmVirtualNetworkPeering](xref:ResourceManager/AzureRM.Network/v3.1.0/Set-AzureRmVirtualNetworkPeering.md)


