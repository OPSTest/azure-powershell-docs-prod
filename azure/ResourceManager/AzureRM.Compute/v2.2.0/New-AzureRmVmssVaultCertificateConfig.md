---
external help file: Microsoft.Azure.Commands.Compute.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: A052C39E-360C-4576-94C8-7EAD4D78CBEC
updated_at: 11/2/2016 6:42 PM
ms.date: 11/2/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.2.0/New-AzureRmVmssVaultCertificateConfig.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/0d1ee921ec0c6fb1faa9cd0f2e2d4c405c1a538a/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.2.0/New-AzureRmVmssVaultCertificateConfig.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: ResourceManager_AzureRM_Compute_v2_2_0_New_AzureRmVmssVaultCertificateConfig_md
---

# New-AzureRmVmssVaultCertificateConfig

## SYNOPSIS
Creates a Key Vault certificate configuration.

## SYNTAX

```
New-AzureRmVmssVaultCertificateConfig [[-CertificateUrl] <String>] [[-CertificateStore] <String>]
 [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureRmVmssVaultCertificateConfig** cmdlet specifies the secret that needs to be placed on the Virtual Machine Scale Set (VMSS) virtual machines.
The output of this cmdlet is intended to be used with the Add-AzureRmVmssSecret cmdlet.

## EXAMPLES

### Example 1: Create a Key Vault certificate configuration
```
PS C:\>New-AzureRmVmssVaultCertificateConfig -CertificateUrl "http://keyVaultName.vault.contoso.net/secrets/secretName/secretVersion" -CertificateStore "MyCerts"
```

This command creates a Key Vault certificate configuration that uses the certificate store named MyCerts located at the specified certificate URL.

## PARAMETERS

### -CertificateStore
Specifies the certificate store on the virtual machines in the scale set where the certificate is added.
This is only valid for Windows Virtual Machine Scale Sets.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -CertificateUrl
Specifies the URI of a certificate stored in the Key Vault.

It is the base64 encoding of the following JSON Object which is encoded in UTF-8:


{
  "data":"\<Base64-encoded-certificate\>",
  "dataType":"pfx",
  "password":"\<pfx-file-password\>"
}

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

###  
This cmdlet does not generate any output.

## NOTES

## RELATED LINKS

[Add-AzureRmVmssSecret](xref:ResourceManager/AzureRM.Compute/v2.2.0/Add-AzureRmVmssSecret.md)
