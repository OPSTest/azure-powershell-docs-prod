---
external help file: Microsoft.Azure.Commands.Dns.dll-Help.xml
ms.assetid: B78F3E8B-C7D2-458C-AB23-06F584FE97E0
online version: 
schema: 2.0.0
updated_at: 1/20/2017 9:17 PM
ms.date: 1/20/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.DNS/v2.5.0/New-AzureRmDnsZone.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.DNS/v2.5.0/New-AzureRmDnsZone.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/cb06bb906911a2a2e1f57adbafe0c0c97a0b205b/azureps-cmdlets-docs/ResourceManager/AzureRM.DNS/v2.5.0/New-AzureRmDnsZone.md
ms.topic: reference
ms.prod: powershell
ms.technology: Azure PowerShell
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: False
ms.service: azure-powershell
---

# New-AzureRmDnsZone

## SYNOPSIS
Creates a new DNS zone.

## SYNTAX

```
New-AzureRmDnsZone -Name <String> -ResourceGroupName <String> [-Tag <Hashtable>] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureRmDnsZone** cmdlet creates a new Domain Name System (DNS) zone in the specified resource group.
You must specify a unique DNS zone name for the *Name* parameter or the cmdlet will return an error.
After the zone is created, use the New-AzureRmDnsRecordSet cmdlet to create record sets in the zone.

You can use the *Confirm* parameter and $ConfirmPreference Windows PowerShell variable to control whether the cmdlet prompts you for confirmation.

## EXAMPLES

### Example 1: Create a DNS zone
```
PS C:\>$Zone = New-AzureRmDnsZone -Name "myzone.com" -ResourceGroupName "MyResourceGroup"
```

This command creates a new DNS zone named myzone.com in the specified resource group, and then stores it in the $Zone variable.

## PARAMETERS

### -Name
Specifies the name of the DNS zone to create.

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
Specifies the resource group in which to create the zone.

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

### -Tag
Specifies an array of tags to associate with the DNS zone.
Tags are name-value pairs represented as hash tables, for example, @(@{"Name"="dept"; "Value"="shopping"}, @{"Name"="env"; "Value"="production"})

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases: Tags

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
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

### -WhatIf
Shows what would happen if the cmdlet runs. The cmdlet is not run.Shows what would happen if the cmdlet runs. The cmdlet is not run.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None
You cannot pipe input to this cmdlet.

## OUTPUTS

### Microsoft.Azure.Commands.Dns.DnsZone
This cmdlet returns an object that represents the new DNS zone.

## NOTES
You can use the *Confirm* parameter to control whether this cmdlet prompts you for confirmation.
By default, the cmdlet prompts you for confirmation if the $ConfirmPreference Windows PowerShell variable has a value of Medium or lower.

If you specify *Confirm* or *Confirm:$True*, this cmdlet prompts you for confirmation before it runs.
If you specify *Confirm:$False*, the cmdlet does not prompt you for confirmation.

## RELATED LINKS

[Get-AzureRmDnsZone](xref:ResourceManager/AzureRM.DNS/v2.5.0/Get-AzureRmDnsZone.md)

[New-AzureRmDnsRecordSet](xref:ResourceManager/AzureRM.DNS/v2.5.0/New-AzureRmDnsRecordSet.md)

[Remove-AzureRmDnsZone](xref:ResourceManager/AzureRM.DNS/v2.5.0/Remove-AzureRmDnsZone.md)
