---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version: .\Get-AzureRmVirtualNetwork.md
schema: 2.0.0
ms.assetid: 779D254B-36A0-42B0-A9CA-39CCCFC257F2
updated_at: 10/31/2016 9:17 PM
ms.date: 10/31/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v2.1.0/Set-AzureRmVirtualNetwork.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/70d99f0e924efe152eb73454f7898f92d5a5db64/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v2.1.0/Set-AzureRmVirtualNetwork.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Set-AzureRmVirtualNetwork

## SYNOPSIS
Sets the goal state for a virtual network.

## SYNTAX

```
Set-AzureRmVirtualNetwork -VirtualNetwork <PSVirtualNetwork> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureRmVirtualNetwork** cmdlet sets the goal state for an Azure virtual network.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -VirtualNetwork
Specifies a **VirtualNetwork** object that represents the goal state.

```yaml
Type: PSVirtualNetwork
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
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

[Get-AzureRmVirtualNetwork](xref:ResourceManager/AzureRM.Network/v2.1.0/Get-AzureRmVirtualNetwork.md)

[Get-AzureRmVirtualNetwork](xref:ResourceManager/AzureRM.Network/v2.1.0/Get-AzureRmVirtualNetwork.md)

[New-AzureRmVirtualNetwork](xref:ResourceManager/AzureRM.Network/v2.1.0/New-AzureRmVirtualNetwork.md)

[Remove-AzureRmVirtualNetwork](xref:ResourceManager/AzureRM.Network/v2.1.0/Remove-AzureRmVirtualNetwork.md)


