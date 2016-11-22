---
external help file: azuread.help.xml
online version: https://blogs.technet.microsoft.com/enterprisemobility/2016/07/18/azuread-certificate-based-authentication-for-ios-and-android-now-in-preview/
schema: 2.0.0
updated_at: 11/21/2016 8:09 PM
ms.date: 11/21/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/live/Azure%20AD%20Cmdlets/AzureAD/v2/New-AzureADTrustedCertificateAuthority.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/e79870303c4a5b18f88c61a5fe206bd45af8c480/Azure%20AD%20Cmdlets/AzureAD/v2/New-AzureADTrustedCertificateAuthority.md
ms.topic: reference
ms.prod: 
ms.service: active-directory
ms.technology: Azure PowerShell
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: carolz
id: AzureAD_v2_New_AzureADTrustedCertificateAuthority_md
---

# New-AzureADTrustedCertificateAuthority

## SYNOPSIS

## SYNTAX

```
New-AzureADTrustedCertificateAuthority -CertificateAuthorityInformation <CertificateAuthorityInformation>
```

## DESCRIPTION

## EXAMPLES

### Create a new Trusted Certificate Authority
```
$cert=Get-Content -Encoding byte â€œ[LOCATION OF THE CER FILE FOR THE CERTIFICATE AUTHORITY]â€
$new_ca=New-Object -TypeName Microsoft.Open.AzureAD.Model.CertificateAuthorityInformation
$new_ca.AuthorityType=0
$new_ca.TrustedCertificate=$cert
$new_ca. crlDistributionPoint = â€œ[URL FOR THE CERTIFICATE REVOCATION LIST]â€
New-AzureADTrustedCertificateAuthority -CertificateAuthorityInformation $new_ca
```

## PARAMETERS

### -CertificateAuthorityInformation
@{Text=}

```yaml
Type: CertificateAuthorityInformation
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByValue, ByPropertyName)
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[More information about the steps to create a trusted certificate authority can be found here:](https://blogs.technet.microsoft.com/enterprisemobility/2016/07/18/azuread-certificate-based-authentication-for-ios-and-android-now-in-preview/)

