---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: .\Add-AzureInternalLoadBalancer.md
schema: 2.0.0
ms.assetid: DFE718B2-4F75-45EA-BCC9-DFBDF4402ADC
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v1.6.1/Remove-AzureInternalLoadBalancer.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v1.6.1/Remove-AzureInternalLoadBalancer.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: 
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Remove-AzureInternalLoadBalancer

## SYNOPSIS
Removes an internal load balancer configuration.

## SYNTAX

```
Remove-AzureInternalLoadBalancer [-ServiceName] <String> [-Profile <AzureSMProfile>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureInternalLoadBalancer** cmdlet removes the internal load balancer configuration from an azure_2 service.
If any endpoint currently refers to the internal load balancer, this cmdlet cannot remove the configuration.

## EXAMPLES

### Example 1: Remove an internal load balancer configuration
```
PS C:\>Remove-AzureInternalLoadBalancer -ServiceName "ContosoService"
```

This command removes the internal load balancer configuration for the service named ContosoService.

## PARAMETERS

### -ServiceName
Specifies the name of the service from which this cmdlet removes an internal load balancer.

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

### -InformationAction
@{Text=}

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
@{Text=}

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

[Add-AzureInternalLoadBalancer](xref:ServiceManagement/Azure.Service/v1.6.1/Add-AzureInternalLoadBalancer.md)

[Get-AzureInternalLoadBalancer](xref:ServiceManagement/Azure.Service/v1.6.1/Get-AzureInternalLoadBalancer.md)

[New-AzureInternalLoadBalancerConfig](xref:ServiceManagement/Azure.Service/v1.6.1/New-AzureInternalLoadBalancerConfig.md)

[Set-AzureInternalLoadBalancer](xref:ServiceManagement/Azure.Service/v1.6.1/Set-AzureInternalLoadBalancer.md)


