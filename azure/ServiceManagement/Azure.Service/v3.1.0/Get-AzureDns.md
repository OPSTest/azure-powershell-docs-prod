---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
ms.assetid: F65D3505-9B07-457B-B3AF-48CB1F5BBA4B
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v3.1.0/Get-AzureDns.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v3.1.0/Get-AzureDns.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureDns

## SYNOPSIS
Gets the DNS settings for an Azure deployment.

## SYNTAX

```
Get-AzureDns [-DnsSettings <DnsSettings>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureDns** cmdlet gets the DNS settings for an Azure deployment.
The cmdlet returns the friendly name and IP address of the DNS server in a DNS settings object.

## EXAMPLES

### Example 1: Get DNS settings
```
PS C:\>Get-AzureDeployment -ServiceName "ContosoService" -Slot "Production" | Get-AzureDNS
```

This command uses the Get-AzureDeployment cmdlet to get the production deployment of the service named ContosoService.
The command passes that object to the current cmdlet by using the pipeline operator.
The current cmdlet gets the DNS settings.

## PARAMETERS

### -DnsSettings
Specifies a **DnsSettings** object.

```yaml
Type: DnsSettings
Parameter Sets: (All)
Aliases: InputObject

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

[Add-AzureDns](xref:ServiceManagement/Azure.Service/v3.1.0/Add-AzureDns.md)

[Get-AzureDeployment](xref:ServiceManagement/Azure.Service/v3.1.0/Get-AzureDeployment.md)

[New-AzureDns](xref:ServiceManagement/Azure.Service/v3.1.0/New-AzureDns.md)

[Remove-AzureDns](xref:ServiceManagement/Azure.Service/v3.1.0/Remove-AzureDns.md)

[Set-AzureDns](xref:ServiceManagement/Azure.Service/v3.1.0/Set-AzureDns.md)


