---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: A15ED498-99D1-4D81-983F-387466C0B904
updated_at: 11/1/2016 10:24 PM
ms.date: 11/1/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v1.6.1/Remove-AzureDns.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/f59f3ef60bc592383812213e69fd77ba950759ed/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v1.6.1/Remove-AzureDns.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Remove-AzureDns

## SYNOPSIS
Removes a DNS server from an Azure service.

## SYNTAX

```
Remove-AzureDns [-Name] <String> [-ServiceName] <String> [-Force] [-Profile <AzureSMProfile>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureDns** cmdlet removes a DNS server from an Azure service.

## EXAMPLES

### Example 1: Remove a DNS server from a service
```
PS C:\>Remove-AzureDns -ServiceName "ContosoService" -Name "Dns07"
```

This command removes the DNS server named Dns07 from ContosoService.

## PARAMETERS

### -Name
Specifies the name of the DNS server that this cmdlet removes.

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

### -ServiceName
Specifies the name of the service from which this cmdlet removes a DNS server.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
ps_force

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
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

### Microsoft.WindowsAzure.Commands.Utilities.Common.ManagementOperationContext

## NOTES

## RELATED LINKS

[Add-AzureDns](xref:ServiceManagement/Azure.Service/v1.6.1/Add-AzureDns.md)

[Get-AzureDns](xref:ServiceManagement/Azure.Service/v1.6.1/Get-AzureDns.md)

[New-AzureDns](xref:ServiceManagement/Azure.Service/v1.6.1/New-AzureDns.md)

[Set-AzureDns](xref:ServiceManagement/Azure.Service/v1.6.1/Set-AzureDns.md)


