---
external help file: Microsoft.Azure.Commands.KeyVault.dll-Help.xml
ms.assetid: 4C40DAC9-5C0B-4AFD-9BDB-D407E0B9F701
online version: 
schema: 2.0.0
updated_at: 1/11/2017 9:26 PM
ms.date: 1/11/2017
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.KeyVault/v2.4.0/New-AzureRmKeyVault.md
original_content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.KeyVault/v2.4.0/New-AzureRmKeyVault.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/cf5fb15dcd1fe2c86458f47e1a11dc88817021fc/azureps-cmdlets-docs/ResourceManager/AzureRM.KeyVault/v2.4.0/New-AzureRmKeyVault.md
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

# New-AzureRmKeyVault

## SYNOPSIS
Creates a key vault.

## SYNTAX

```
New-AzureRmKeyVault [-VaultName] <String> [-ResourceGroupName] <String> [-Location] <String>
 [-EnabledForDeployment] [-EnabledForTemplateDeployment] [-EnabledForDiskEncryption] [-Sku <SkuName>]
 [-Tag <Hashtable>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureRmKeyVault** cmdlet creates a key vault in the specified resource group.
This cmdlet also grants permissions to the currently logged on user to add, remove, or list keys and secrets in the key vault.

Note: If you see the error **The subscription is not registered to use namespace 'Microsoft.KeyVault'** when you try to create your new key vault, run **Register-AzureRmResourceProvider -ProviderNamespace "Microsoft.KeyVault"** and then rerun your **New-AzureRmKeyVault** command.
For more information, see Register-AzureRmResourceProvider.

## EXAMPLES

### Example 1: Create a Standard key vault
```
PS C:\>New-AzureRmKeyVault -VaultName 'Contoso03Vault' -ResourceGroupName 'Group14' -Location 'East US'
```

This command creates a key vault named Contoso03Vault, in the Azure region East US.
The command adds the key vault to the resource group named Group14.
Because the command does not specify a value for the *SKU* parameter, it creates a Standard key vault.

### Example 2: Create a Premium key vault
```
PS C:\>New-AzureRmKeyVault -VaultName 'Contoso03Vault' -ResourceGroupName 'Group14' -Location 'East US' -Sku 'Premium'
```

This command creates a key vault, just like the previous example.
However, it specifies a value of Premium for the *SKU* parameter to create a Premium key vault.

## PARAMETERS

### -EnabledForDeployment
Enables the Microsoft.Compute resource provider to retrieve secrets from this key vault when this key vault is referenced in resource creation, for example when creating a virtual machine.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -EnabledForDiskEncryption
Enables the Azure disk encryption service to get secrets and unwrap keys from this key vault.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -EnabledForTemplateDeployment
Enables Azure Resource Manager to get secrets from this key vault when this key vault is referenced in a template deployment.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Location
Specifies the Azure region in which to create the key vault.
Use the command Get-AzureLocationhttps://msdn.microsoft.com/ library/azure/mt589064.aspx to see your choices.
For more information, type `Get-Help Get-AzureLocation`.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of an existing resource group in which to create the key vault.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Sku
Specifies the SKU of the key vault instance.
For information about which features are available for each SKU, see the Azure Key Vault Pricinghttp://go.microsoft.com/fwlink/?linkid=512521 website (http://go.microsoft.com/fwlink/?linkid=512521).

```yaml
Type: SkuName
Parameter Sets: (All)
Aliases: 
Accepted values: Standard, Premium

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Tag
Specifies a hash table that represents resource tags.

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases: Tags

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -VaultName
Specifies the name of the key vault to create.
The name can be any combination of letters, digits, or hyphens.
The name must start and end with a letter or digit.
The name must be universally unique.

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

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.Azure.Commands.KeyVault.Models.PSVault

## NOTES

## RELATED LINKS

[Get-AzureRmKeyVault](xref:ResourceManager/AzureRM.KeyVault/v2.4.0/Get-AzureRmKeyVault.md)

[Remove-AzureRmKeyVault](xref:ResourceManager/AzureRM.KeyVault/v2.4.0/Remove-AzureRmKeyVault.md)
