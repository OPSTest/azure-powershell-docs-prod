---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 2A35B1DA-9917-4754-9C56-EF6993DC6E9A
updated_at: 11/1/2016 10:24 PM
ms.date: 11/1/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v0.9.8/Add-AzureCertificate.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v0.9.8/Add-AzureCertificate.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/f59f3ef60bc592383812213e69fd77ba950759ed/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v0.9.8/Add-AzureCertificate.md
ms.topic: reference
ms.prod: powershell
ms.technology: Azure PowerShell
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: erickson-doug
open_to_public_contributors: False
ms.service: azure-powershell
---

# Add-AzureCertificate

## SYNOPSIS
Uploads a certificate to an Azure cloud service.

## SYNTAX

```
Add-AzureCertificate [-ServiceName] <String> [-CertToDeploy] <Object> [-Password <String>]
 [-Profile <AzureProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Add-AzureCertificate** cmdlet uploads a certificate for an Azure service.

## EXAMPLES

### Example 1: Upload a certificate and password
```
PS C:\>Add-AzureCertificate -ServiceName "ContosoService" -CertToDeploy ContosoCertificate.pfx -Password "password"
```

This command uploads the certificate file ContosoCertificate.pfx to a cloud service.
The command specifies the password for the certificate.

### Example 2: Upload a certificate file
```
PS C:\>Add-AzureCertificate -serviceName "MyService" -CertToDeploy ContosoCertificate.cer
```

This command uploads the certificate file ContosoCertificate.cer to a cloud service.
The command specifies the password for the certificate.

### Example 3: Upload a certificate object
```
PS C:\>$Certificate = Get-Item cert:\PATTIFULLER\MY\1D6E34B526723E06C235BE8E5457784BF12C9F39
PS C:\> Add-AzureCertificate -ServiceName "ContosoService" -CertToDeploy $Certificate
```

The first command gets a certificate from the MY store of a user by using the Windows PowerShell core Get-Item cmdlet.
The command stores the certificate in the $Certificate variable.

The second command uploads the certificate in $certificate to a cloud service.

## PARAMETERS

### -ServiceName
Specifies the name of the Azure service to which this cmdlet adds a certificate.

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

### -CertToDeploy
Specifies the certificate to deploy.
You can specify the full path of a certificate file, such as a file that has a *.cer or *.
pfx file name extension, or an X.509 Certificate object.

```yaml
Type: Object
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Password
Specifies the certificate password.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Profile
Specifies the Azure profile from which this cmdlet reads.
If you do not specify a profile, this cmdlet reads from the local default profile.

```yaml
Type: AzureProfile
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

### ManagementOperationContext

## NOTES

## RELATED LINKS

[Get-AzureCertificate](xref:ServiceManagement/Azure.Service/v0.9.8/Get-AzureCertificate.md)

[New-AzureCertificateSetting](xref:ServiceManagement/Azure.Service/v0.9.8/New-AzureCertificateSetting.md)

[Remove-AzureCertificate](xref:ServiceManagement/Azure.Service/v0.9.8/Remove-AzureCertificate.md)


