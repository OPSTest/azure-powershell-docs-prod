---
external help file: Microsoft.Azure.Commands.KeyVault.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkID=826271
schema: 2.0.0
updated_at: 10/14/2016 7:06 AM
ms.date: 10/14/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.KeyVault/v2.0/CmdletMDs/Get-AzureKeyVaultCertificateIssuer.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/a56d0e01e65c2c33aa2af13dd29addc94ead6e88/azureps-cmdlets-docs/ResourceManager/AzureRM.KeyVault/v2.0/CmdletMDs/Get-AzureKeyVaultCertificateIssuer.md
ms.topic: reference
ms.prod: powershell
ms.service: Azure PowerShell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureKeyVaultCertificateIssuer

## SYNOPSIS
Gets a certificate issuer for a key vault.

## SYNTAX

### ByVaultName (Default)
```
Get-AzureKeyVaultCertificateIssuer [-VaultName] <String> [<CommonParameters>]
```

### ByName
```
Get-AzureKeyVaultCertificateIssuer [-VaultName] <String> [-Name] <String> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureKeyVaultCertificateIssuer** cmdlet gets a specified certificate issuer or all certificate issuers for a key vault in Azure Key Vault.

## EXAMPLES

### Example 1: Get a certificate issuer
```
PS C:\>Get-AzureKeyVaultCertificateIssuer -VaultName "Contosokv01" -Name "TestIssuer01"
Name                : TestIssuer01
IssuerProvider      : Test
AccountId           : 555
ApiKey              : 
OrganizationDetails : Microsoft.Azure.Commands.KeyVault.Models.KeyVaultCertificateOrganizationDetails
```

This command gets the certificate issuer named TestIssuer01.

## PARAMETERS

### -Name
Specifies the name of the certificate issuer to get.

```yaml
Type: String
Parameter Sets: ByName
Aliases: IssuerName

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -VaultName
Specifies the name of a key vault.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### List<Microsoft.Azure.Commands.KeyVault.Models.CertificateIssuerIdentityItem>, Microsoft.Azure.Commands.KeyVault.Models.KeyVaultCertificateIssuer

## NOTES

## RELATED LINKS

[Remove-AzureKeyVaultCertificateIssuer](.\Remove-AzureKeyVaultCertificateIssuer.md)

[Set-AzureKeyVaultCertificateIssuer](.\Set-AzureKeyVaultCertificateIssuer.md)
