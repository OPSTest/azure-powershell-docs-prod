---
external help file: Microsoft.WindowsAzure.Commands.TrafficManager.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: D113375A-BE10-458E-9103-7EBC63309259
updated_at: 11/11/2016 11:03 PM
ms.date: 11/11/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ServiceManagement/Azure.TrafficManager/v1.6.1/Test-AzureTrafficManagerDomainName.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/79eeb985ea480979357fb4695832a0c3d29a48bf/azureps-cmdlets-docs/ServiceManagement/Azure.TrafficManager/v1.6.1/Test-AzureTrafficManagerDomainName.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
id: ServiceManagement_Azure_TrafficManager_v1_6_1_Test_AzureTrafficManagerDomainName_md
---

# Test-AzureTrafficManagerDomainName

## SYNOPSIS
Checks whether a domain name is available as a Traffic Manager profile.

## SYNTAX

```
Test-AzureTrafficManagerDomainName [-DomainName] <String> [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Test-AzureTrafficManagerDomainName** cmdlet checks whether a domain name is available as a Microsoft Azure Traffic Manager profile.
If the domain name is available, this cmdlet returns a value of $True.

## EXAMPLES

### Example 1: Check whether a domain name is available
```
PS C:\>Test-AzureTrafficManagerDomainName -DomainName "ContosoApp.trafficmanager.net"
$True
```

This command checks whether the domain name ContosoApp.trafficmanager.net is available as a Traffic Manager profile.

## PARAMETERS

### -DomainName
Specifies the domain name to test.
You must include the following string: 

.trafficmanager.net

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Profile
In-memory profile.

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

### System.Boolean
This cmdlet generates $True or $False.
If the domain name is available, this cmdlet returns a value of $True.

## NOTES

## RELATED LINKS


