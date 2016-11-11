---
external help file: Microsoft.WindowsAzure.Commands.RemoteApp.dll-Help.xml
ms.assetid: 654C490B-1C87-4920-B525-C12DB1152AB1
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ServiceManagement/Azure.RemoteApp/v3.1.0/Rename-AzureRemoteAppTemplateImage.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ServiceManagement/Azure.RemoteApp/v3.1.0/Rename-AzureRemoteAppTemplateImage.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Rename-AzureRemoteAppTemplateImage

## SYNOPSIS
Renames an Azure RemoteApp template image.

## SYNTAX

```
Rename-AzureRemoteAppTemplateImage [-ImageName] <String> [-NewName] <String> [-Profile <AzureSMProfile>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Rename-AzureRemoteAppTemplateImage** cmdlet renames an Azure RemoteApp template image.

## EXAMPLES

### Example 1: Rename a template image
```
PS C:\>Rename-AzureRemoteAppTemplateImage -ImageName "ContosoApps" -NewName "ContosoFinanceApps"
```

This command renames the Azure RemoteApp template image named ContosoApps to ContosoFinanceApps.

## PARAMETERS

### -ImageName
Specifies the name of an Azure RemoteApp template image to rename.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -NewName
Specifies a new name for an Azure RemoteApp template image.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
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

[Get-AzureRemoteAppTemplateImage](xref:ServiceManagement/Azure.RemoteApp/v3.1.0/Get-AzureRemoteAppTemplateImage.md)

[New-AzureRemoteAppTemplateImage](xref:ServiceManagement/Azure.RemoteApp/v3.1.0/New-AzureRemoteAppTemplateImage.md)

[Remove-AzureRemoteAppTemplateImage](xref:ServiceManagement/Azure.RemoteApp/v3.1.0/Remove-AzureRemoteAppTemplateImage.md)


