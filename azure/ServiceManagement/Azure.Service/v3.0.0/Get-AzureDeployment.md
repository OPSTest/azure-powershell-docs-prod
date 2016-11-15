---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 05D5B12E-9FD6-4513-B80C-48ADB5732DCE
updated_at: 11/11/2016 11:03 PM
ms.date: 11/11/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v3.0.0/Get-AzureDeployment.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/79eeb985ea480979357fb4695832a0c3d29a48bf/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v3.0.0/Get-AzureDeployment.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
id: ServiceManagement_Azure_Service_v3_0_0_Get_AzureDeployment_md
---

# Get-AzureDeployment

## SYNOPSIS
Gets details of a deployment.

## SYNTAX

```
Get-AzureDeployment [-ServiceName] <String> [[-Slot] <String>] [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureDeployment** cmdlet gets details of an Azure deployment.
Specify the name of the Azure service and the slot of the deployment.

## EXAMPLES

### Example 1: Get details for a production deployment
```
PS C:\>Get-AzureDeployment -ServiceName "ContosoService"
```

This command returns the details of the deployment for the service named ContosoService.
This command does not specify a slot.
Therefore, the command uses the default value of Production.

### Example 2: Get details for a staging deployment
```
PS C:\>Get-AzureDeployment -ServiceName "ContosoService" -Slot "Staging"
```

This command returns the details of the staging deployment of ContosoService.

## PARAMETERS

### -ServiceName
Specifies the name of the service.

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

### -Slot
Specifies the environment of the deployment.
Valid values are: Staging or Production.
The default value is Production.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Profile
Specifies the Azure profile from which this cmdlet reads.
If you do not specify a profile, this cmdlet reads from the local default profile.

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

## NOTES

## RELATED LINKS

[Get-AzureDeploymentEvent](xref:ServiceManagement/Azure.Service/v3.0.0/Get-AzureDeploymentEvent.md)

[Move-AzureDeployment](xref:ServiceManagement/Azure.Service/v3.0.0/Move-AzureDeployment.md)

[New-AzureDeployment](xref:ServiceManagement/Azure.Service/v3.0.0/New-AzureDeployment.md)

[Remove-AzureDeployment](xref:ServiceManagement/Azure.Service/v3.0.0/Remove-AzureDeployment.md)

[Set-AzureDeployment](xref:ServiceManagement/Azure.Service/v3.0.0/Set-AzureDeployment.md)


