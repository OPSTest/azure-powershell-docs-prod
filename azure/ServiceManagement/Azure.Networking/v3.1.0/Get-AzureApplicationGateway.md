---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.Network.dll-Help.xml
ms.assetid: 75505BF1-69C2-4502-A161-F06527C20D34
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v3.1.0/Get-AzureApplicationGateway.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v3.1.0/Get-AzureApplicationGateway.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: ServiceManagement_Azure_Networking_v3_1_0_Get_AzureApplicationGateway_md
---

# Get-AzureApplicationGateway

## SYNOPSIS
Gets an Application Gateway.

## SYNTAX

```
Get-AzureApplicationGateway [[-Name] <String>] [-Profile <AzureSMProfile>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureApplicationGateway** cmdlet gets an existing Azure Application Gateway.

## EXAMPLES

### Example 1: Get an Application Gateway
```
PS C:\>Get-AzureApplicationGateway -Name "ApplicationGateway06"
```

This command gets the Application Gateway named ApplicationGateway06.

### Example 2: Get all Application Gateways
```
PS C:\>Get-AzureApplicationGateway
```

This command gets all the Application Gateways under your subscription.

## PARAMETERS

### -Name
Specifies the name of the Application Gateway that this cmdlet gets.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Profile
Specifies the Azure profile from which this cmdlet reads. 
If you do not specify a profile, this cmdlet reads from the local default profile.
By default, this cmdlet does not generate any output.

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

### System.String

## OUTPUTS

### Microsoft.Azure.Networking.ApplicationGatewayObjectModel.ApplicationGateway, IEnumerable<Microsoft.Azure.Networking.ApplicationGatewayObjectModel.ApplicationGateway>

## NOTES

## RELATED LINKS

[New-AzureApplicationGateway](xref:ServiceManagement/Azure.Networking/v3.1.0/New-AzureApplicationGateway.md)

[Remove-AzureApplicationGateway](xref:ServiceManagement/Azure.Networking/v3.1.0/Remove-AzureApplicationGateway.md)

[Start-AzureApplicationGateway](xref:ServiceManagement/Azure.Networking/v3.1.0/Start-AzureApplicationGateway.md)

[Stop-AzureApplicationGateway](xref:ServiceManagement/Azure.Networking/v3.1.0/Stop-AzureApplicationGateway.md)

[Update-AzureApplicationGateway](xref:ServiceManagement/Azure.Networking/v3.1.0/Update-AzureApplicationGateway.md)


