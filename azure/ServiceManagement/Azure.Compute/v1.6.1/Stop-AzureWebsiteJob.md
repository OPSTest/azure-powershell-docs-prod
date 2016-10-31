---
external help file: Microsoft.WindowsAzure.Commands.dll-Help.xml
online version: .\Stop-AzureWebsite.md
schema: 2.0.0
ms.assetid: 9698753F-0BFC-4845-B74E-6C6BED38A430
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v1.6.1/Stop-AzureWebsiteJob.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v1.6.1/Stop-AzureWebsiteJob.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Stop-AzureWebsiteJob

## SYNOPSIS
Stops a web job for a website

## SYNTAX

```
Stop-AzureWebsiteJob -JobName <String> [-PassThru] [[-Name] <String>] [-Slot <String>]
 [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
Stops a web job for a website

## EXAMPLES

### --------------  Stop a web job for a website --------------
```
C:\PS>Stop-AzureWebsiteJob -Name MyWebsite -JobName MyWebJob -JobType Continuous
```

Stops a web job called MyWebJob for MyWebSite

## PARAMETERS

### -Name
The name of the Azure website

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Slot
The slot name of the Azure website

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -JobName
The web job name

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

### -PassThru
Returns a boolean value indicating that the job stopped successfully.
By default, this cmdlet does not return any output.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
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

## NOTES

## RELATED LINKS

[Stop-AzureWebsite](xref:ServiceManagement/Azure.Compute/v1.6.1/Stop-AzureWebsite.md)

[Get-AzureWebsiteJob](xref:ServiceManagement/Azure.Compute/v1.6.1/Get-AzureWebsiteJob.md)

[New-AzureWebsiteJob](xref:ServiceManagement/Azure.Compute/v1.6.1/New-AzureWebsiteJob.md)

[Remove-AzureWebsiteJob](xref:ServiceManagement/Azure.Compute/v1.6.1/Remove-AzureWebsiteJob.md)

[Start-AzureWebsiteJob](xref:ServiceManagement/Azure.Compute/v1.6.1/Start-AzureWebsiteJob.md)


