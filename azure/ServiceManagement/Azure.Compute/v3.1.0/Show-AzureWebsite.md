---
external help file: Microsoft.WindowsAzure.Commands.dll-Help.xml
ms.assetid: 7785F288-1CDF-444E-B72F-597E75B76074
online version: 
schema: 2.0.0
updated_at: 11/11/2016 11:03 PM
ms.date: 11/11/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v3.1.0/Show-AzureWebsite.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/79eeb985ea480979357fb4695832a0c3d29a48bf/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v3.1.0/Show-AzureWebsite.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: ServiceManagement_Azure_Compute_v3_1_0_Show_AzureWebsite_md
---

# Show-AzureWebsite

## SYNOPSIS
Opens a browser on a specified website.

## SYNTAX

```
Show-AzureWebsite [[-Name] <String>] [-Slot <String>] [-Profile <AzureSMProfile>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
This topic describes the cmdlet in the 0.8.10 version of the Microsoft Azure PowerShell module.
To get the version of the module you're using, in the Azure PowerShell console, type (Get-Module -Name Azure).Version.

The **Show-AzureWebsite** cmdlet opens a browser on a specified website.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -Name
Specifies the name of the site to open in the browser.

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

### -Slot
Specifies the slot name of the website.

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

[Show-AzurePortal](xref:ServiceManagement/Azure.Compute/v3.1.0/Show-AzurePortal.md)

[Get-AzureWebsite](xref:ServiceManagement/Azure.Compute/v3.1.0/Get-AzureWebsite.md)

[New-AzureWebsite](xref:ServiceManagement/Azure.Compute/v3.1.0/New-AzureWebsite.md)

[Remove-AzureWebsite](xref:ServiceManagement/Azure.Compute/v3.1.0/Remove-AzureWebsite.md)

[Restart-AzureWebsite](xref:ServiceManagement/Azure.Compute/v3.1.0/Restart-AzureWebsite.md)

[Set-AzureWebsite](xref:ServiceManagement/Azure.Compute/v3.1.0/Set-AzureWebsite.md)


