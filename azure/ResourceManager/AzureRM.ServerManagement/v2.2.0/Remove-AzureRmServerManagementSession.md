---
external help file: Microsoft.Azure.Commands.ServerManagement.dll-Help.xml
online version: bcd0e4a3-8586-4fd6-8ef7-35f5e14fcfcb
schema: 2.0.0
ms.assetid: 0685B321-0FE4-4760-9446-17656F9DB600
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.ServerManagement/v2.2.0/Remove-AzureRmServerManagementSession.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.ServerManagement/v2.2.0/Remove-AzureRmServerManagementSession.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: 
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Remove-AzureRmServerManagementSession

## SYNOPSIS
Removes a Server Management session.

## SYNTAX

### ByName
```
Remove-AzureRmServerManagementSession [-ResourceGroupName] <String> [-NodeName] <String>
 [-SessionName] <String> [<CommonParameters>]
```

### ByObject
```
Remove-AzureRmServerManagementSession [[-SessionName] <String>] [-Session] <Session> [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRmServerManagementSession** cmdlet removes an Azure Server Management session.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -ResourceGroupName
Specifies the name of the resource group that the session belongs to.

```yaml
Type: String
Parameter Sets: ByName
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -NodeName
Specifies the name of the node on which this cmdlet removes the session.

```yaml
Type: String
Parameter Sets: ByName
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -SessionName
Specifies the name of the session that this cmdlet removes.

```yaml
Type: String
Parameter Sets: ByName
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

```yaml
Type: String
Parameter Sets: ByObject
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Session
Specifies the session that this cmdlet removes.

This parameter may be used instead of the *ResourceGroupName*, *NodeName* and *SessionName* parameters.

```yaml
Type: Session
Parameter Sets: ByObject
Aliases: 

Required: True
Position: 0
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

[Get-AzureRmServerManagementSession](xref:ResourceManager/AzureRM.ServerManagement/v2.2.0/Get-AzureRmServerManagementSession.md)

[New-AzureRmServerManagementSession](xref:ResourceManager/AzureRM.ServerManagement/v2.2.0/New-AzureRmServerManagementSession.md)


