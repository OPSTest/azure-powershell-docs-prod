---
external help file: Microsoft.Azure.Commands.ApiManagement.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 73F73A6F-470C-4DD6-95C4-A1302FABB0DD
updated_at: 11/1/2016 10:24 PM
ms.date: 11/1/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/v2.1.0/New-AzureRmApiManagementHostnameConfiguration.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/f59f3ef60bc592383812213e69fd77ba950759ed/azureps-cmdlets-docs/ResourceManager/AzureRM.ApiManagement/v2.1.0/New-AzureRmApiManagementHostnameConfiguration.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# New-AzureRmApiManagementHostnameConfiguration

## SYNOPSIS
Creates an instance of PsApiManagementHostnameConfiguration.

## SYNTAX

```
New-AzureRmApiManagementHostnameConfiguration -CertificateThumbprint <String> -Hostname <String>
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureRmApiManagementHostnameConfiguration** cmdlet is a helper command that creates an instance of **PsApiManagementHostnameConfiguration**.
This command is used with the Set-AzureRmApiManagementHostnames cmdlet.

## EXAMPLES

### Example 1: Create and initialize an instance of PsApiManagementHostnameConfiguration
```
PS C:\>New-AzureRmApiManagementHostnameConfiguration -Hostname "portal.contoso.com" -CertificateThumbprint "33CC47C6FCA848DC9B14A6F071C1EF7C"
```

This command creates and initializes an instance of **PsApiManagementHostnameConfiguration**.

## PARAMETERS

### -CertificateThumbprint
Specifies the certificate thumbprint.
The certificate must be first imported with the Import-AzureRmApiManagementHostnameCertificate cmdlet.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Hostname
Specifies the custom host name for which this cmdlet creates the **PsApiManagementHostnameConfiguration** instance.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
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

[Import-AzureRmApiManagementHostnameCertificate](xref:ResourceManager/AzureRM.ApiManagement/v2.1.0/Import-AzureRmApiManagementHostnameCertificate.md)

[Set-AzureRmApiManagementHostnames](xref:ResourceManager/AzureRM.ApiManagement/v2.1.0/Set-AzureRmApiManagementHostnames.md)


