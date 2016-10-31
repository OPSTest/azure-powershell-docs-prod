---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: .\Add-AzureDns.md
schema: 2.0.0
ms.assetid: DB18688F-188C-49CE-AD9D-8D4BC1F09AF7
updated_at: 10/31/2016 9:17 PM
ms.date: 10/31/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v1.6.1/New-AzureDns.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/70d99f0e924efe152eb73454f7898f92d5a5db64/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v1.6.1/New-AzureDns.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# New-AzureDns

## SYNOPSIS
Creates an Azure DNS settings object.

## SYNTAX

```
New-AzureDns [-Name] <String> [-IPAddress] <String> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureDns** cmdlet creates an Azure DNS settings object.
You can use a DNS settings object when you create a virtual machine by using the New-AzureVM cmdlet.

## EXAMPLES

### Example 1: Create a DNS settings object
```
PS C:\>$Dns = New-AzureDns -Name "Dns01" -IPAddress "10.1.2.4"
```

This command creates an Azure DNS settings object.
The DNS server has the specified address and the friendly name Dns01.
The command stores the object in the $Dns variable for use by the **New-AzureVM** cmdlet.

## PARAMETERS

### -Name
Specifies a friendly name for the DNS server.
This name is not necessarily a fully qualified domain name.

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

### -IPAddress
Specifies the IP address of the DNS server.

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

[Add-AzureDns](xref:ServiceManagement/Azure.Service/v1.6.1/Add-AzureDns.md)

[Get-AzureDns](xref:ServiceManagement/Azure.Service/v1.6.1/Get-AzureDns.md)

[New-AzureVM](xref:ServiceManagement/Azure.Service/v1.6.1/New-AzureVM.md)

[Remove-AzureDns](xref:ServiceManagement/Azure.Service/v1.6.1/Remove-AzureDns.md)

[Set-AzureDns](xref:ServiceManagement/Azure.Service/v1.6.1/Set-AzureDns.md)


