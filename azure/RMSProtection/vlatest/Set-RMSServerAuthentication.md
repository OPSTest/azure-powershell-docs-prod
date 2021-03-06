---
external help file: RMSProtection.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkID=623208
schema: 2.0.0
ms.assetid: B46B757C-DF4D-4BCE-9732-527A86498619
updated_at: 1/13/2017 11:09 PM
ms.date: 1/13/2017
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/Azure%20Information%20Protection/RMSProtection/vlatest/Set-RMSServerAuthentication.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/Azure%20Information%20Protection/RMSProtection/vlatest/Set-RMSServerAuthentication.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/73fede5be8d73e5de67a785007346f27b5795709/Azure%20Information%20Protection/RMSProtection/vlatest/Set-RMSServerAuthentication.md
ms.topic: reference
ms.prod: powershell
ms.technology: Azure Powershell
author: cabailey
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: cabailey
open_to_public_contributors: False
ms.service: rights-management
---

# Set-RMSServerAuthentication

## SYNOPSIS
Sets the service principal authentication credentials for Azure RMS.

## SYNTAX

```
Set-RMSServerAuthentication -Key <String> -AppPrincipalId <String> -BposTenantId <String> [<CommonParameters>]
```

## DESCRIPTION
The **Set-RMSServerAuthentication** cmdlet specifies identifiers for a service principal to authenticate with Azure RMS, so that you can then protect or unprotect files by using Azure RMS. Use a service principal when you need to protect or unprotect files without interaction, for example, a script that automatically protects files on a file server. You need run this command just one time for your Windows PowerShell session.

This cmdlet is for Azure RMS only and is not used for AD RMS. This cmdlet also does not apply if you are authenticating to Azure RMS by using your user account. For more information about this cmdlet and how to get the identifiers that it requires, see [about_RMSProtection_AzureRMS](http://go.microsoft.com/fwlink/?LinkId=620287).

## EXAMPLES

### Example 1: Set the service principal authentication credentials for Azure RMS
```
PS C:\>Set-RMSServerAuthentication -BposTenantId "23976bc6-dcd4-4173-9d96-dad1f48efd42" -Key "zIeMu8zNJ6U377CLtppkhkbl4gjodmYSXUVwAO5ycgA=" -AppPrincipalId "b5e3f76a-b5c2-4c96-a594-a0807f65bba4"
The RmsServerAuthentication is set to ON
```

This command sets the service principle authentication credentials for Azure RMS, by specifying the required three identifiers for a previously created service principal.

## PARAMETERS

### -AppPrincipalId
Specifies the AppPrincipalId value of the service principal.

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

### -BposTenantId
Specifies the BposTenantId value (the tenant ID) to which the service principal belongs.

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

### -Key
Specifies the symmetric key value for the service principal.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-RMSServerAuthentication](xref:RMSProtection/vlatest/Get-RMSServerAuthentication.md)
