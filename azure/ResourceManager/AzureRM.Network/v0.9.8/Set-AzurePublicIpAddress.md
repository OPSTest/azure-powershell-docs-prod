---
external help file: Microsoft.Azure.Commands.Network.dll-Help.xml
online version: .\Get-AzurePublicIpAddress.md
schema: 2.0.0
ms.assetid: A2DE176B-584B-4FDD-8591-F4FD44045BB2
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v0.9.8/Set-AzurePublicIpAddress.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Network/v0.9.8/Set-AzurePublicIpAddress.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: PowerShellHelpPub
---

# Set-AzurePublicIpAddress

## SYNOPSIS
Sets the goal state for a public IP address.

## SYNTAX

```
Set-AzurePublicIpAddress -PublicIpAddress <PSPublicIpAddress> [-Profile <AzureProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzurePublicIpAddress** cmdlet sets the goal state for a public IP address.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -Profile
Specifies an Azure profile.

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

### -PublicIpAddress
Specifis a **PublicIpAddress** object that represents the goal state to which the public IP address should be set.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzurePublicIpAddress](./Get-AzurePublicIpAddress.md)

[New-AzurePublicIpAddress](./New-AzurePublicIpAddress.md)

[Remove-AzurePublicIpAddress](./Remove-AzurePublicIpAddress.md)


