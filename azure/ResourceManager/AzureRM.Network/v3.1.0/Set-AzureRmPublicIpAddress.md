---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
ms.assetid: EC798838-1850-4E88-B17F-D2F00F2D4EE9
online version: 
schema: 2.0.0
updated_at: 11/11/2016 11:03 PM
ms.date: 11/11/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.1.0/Set-AzureRmPublicIpAddress.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/79eeb985ea480979357fb4695832a0c3d29a48bf/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v3.1.0/Set-AzureRmPublicIpAddress.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: ResourceManager_AzureRM_Network_v3_1_0_Set_AzureRmPublicIpAddress_md
---

# Set-AzureRmPublicIpAddress

## SYNOPSIS
Sets the goal state for a public IP address.

## SYNTAX

```
Set-AzureRmPublicIpAddress -PublicIpAddress <PSPublicIpAddress> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureRmPublicIpAddress** cmdlet sets the goal state for a public IP address.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -PublicIpAddress
Specifies a **PublicIpAddress** object that represents the goal state to which the public IP address should be set.

```yaml
Type: PSPublicIpAddress
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

[Get-AzureRmPublicIpAddress](xref:ResourceManager/AzureRM.Network/v3.1.0/Get-AzureRmPublicIpAddress.md)

[Get-AzureRmPublicIpAddress](xref:ResourceManager/AzureRM.Network/v3.1.0/Get-AzureRmPublicIpAddress.md)

[New-AzureRmPublicIpAddress](xref:ResourceManager/AzureRM.Network/v3.1.0/New-AzureRmPublicIpAddress.md)

[Remove-AzureRmPublicIpAddress](xref:ResourceManager/AzureRM.Network/v3.1.0/Remove-AzureRmPublicIpAddress.md)


