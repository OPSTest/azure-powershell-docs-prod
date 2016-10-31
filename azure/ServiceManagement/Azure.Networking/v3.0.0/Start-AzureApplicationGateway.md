---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.Network.dll-Help.xml
online version: 75505bf1-69c2-4502-a161-f06527c20d34
schema: 2.0.0
ms.assetid: C2FB6496-8887-45B9-83C1-1F47EC78B0A6
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v3.0.0/Start-AzureApplicationGateway.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v3.0.0/Start-AzureApplicationGateway.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: 
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Start-AzureApplicationGateway

## SYNOPSIS
Starts an application gateway.

## SYNTAX

```
Start-AzureApplicationGateway [-Name] <String> [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Start-AzureApplicationGateway** cmdlet starts an application gateway.

## EXAMPLES

### Example 1: Start an application gateway
```
PS C:\>Start-AzureApplicationGateway -Name "ApplicationGateway06"
```

This command starts the application gateway named ApplicationGateway06.

## PARAMETERS

### -Name
Specifies the name of the application gateway that this cmdlet starts.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String

## OUTPUTS

### Microsoft.WindowsAzure.Management.ApplicationGateway.Models.ApplicationGatewayOperationResponse

## NOTES

## RELATED LINKS

[Get-AzureApplicationGateway](xref:ServiceManagement/Azure.Networking/v3.0.0/Get-AzureApplicationGateway.md)

[New-AzureApplicationGateway](xref:ServiceManagement/Azure.Networking/v3.0.0/New-AzureApplicationGateway.md)

[Remove-AzureApplicationGateway](xref:ServiceManagement/Azure.Networking/v3.0.0/Remove-AzureApplicationGateway.md)

[Stop-AzureApplicationGateway](xref:ServiceManagement/Azure.Networking/v3.0.0/Stop-AzureApplicationGateway.md)

[Update-AzureApplicationGateway](xref:ServiceManagement/Azure.Networking/v3.0.0/Update-AzureApplicationGateway.md)


