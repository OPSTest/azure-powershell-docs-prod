---
external help file: Microsoft.Azure.Commands.SiteRecovery.dll-Help.xml
online version: 9c88dc0e-618a-4ffa-8e73-8c75783c6fc8
schema: 2.0.0
ms.assetid: 0D000EAB-C592-449E-9150-8D0E4A28BF3D
updated_at: 11/1/2016 9:57 PM
ms.date: 11/1/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.SiteRecovery/v3.1.0/Remove-AzureRmSiteRecoveryServer.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/50b226c3bc01309b65b424d0cf5725cefea50561/azureps-cmdlets-docs/ResourceManager/AzureRM.SiteRecovery/v3.1.0/Remove-AzureRmSiteRecoveryServer.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Remove-AzureRmSiteRecoveryServer

## SYNOPSIS
Removes a Site Recovery server from the current vault.

## SYNTAX

```
Remove-AzureRmSiteRecoveryServer -Server <ASRServer> [-Force] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRmSiteRecoveryServer** cmdlet unregisters an Azure Site Recovery server which removes it from the current vault.

## EXAMPLES


## PARAMETERS

### -Server
Specifies the Site Recovery server object.

```yaml
Type: ASRServer
Parameter Sets: (All)
Aliases:

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Force
Forces the command to run without asking for user confirmation.

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

### -WhatIf
Shows what would happen if the cmdlet runs.

The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmSiteRecoveryServer](xref:ResourceManager/AzureRM.SiteRecovery/v3.1.0/Get-AzureRmSiteRecoveryServer.md)

[Update-AzureRmSiteRecoveryServer](xref:ResourceManager/AzureRM.SiteRecovery/v3.1.0/Update-AzureRmSiteRecoveryServer.md)
