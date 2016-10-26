---
external help file: Microsoft.RightsManagementServices.Online.Admin.PowerShell.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=400592
schema: 2.0.0
ms.assetid: A1C99424-D986-4A5A-B2E1-6D18EEF11B21
updated_at: 10/24/2016 10:52 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/Azure%20Information%20Protection/AADRM%20Module/vlatest/Add-AadrmKey.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/5e6ef5e3f1d6768f64c5d14aab4fd3e58b8fa0c3/Azure%20Information%20Protection/AADRM%20Module/vlatest/Add-AadrmKey.md
ms.topic: reference
ms.prod: powershell
ms.service: rights-management
ms.technology: Azure Powershell
author: visual-studio-china
ms.author: 
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Add-AadrmKey

## SYNOPSIS
Adds a legacy customer-managed tenant key for Rights Management, and makes it the active key.

## SYNTAX

```
Add-AadrmKey [-Force] -KeyFile <String> [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Add-AadrmKey** cmdlet adds a legacy customer-managed tenant key over the Internet to the Azure Rights Management service, and makes that key the active tenant key for your tenant.
The previously active tenant key is archived.

**Note**: This cmdlet is now deprecated because Azure RMS uses Azure Key Vault for customer-managed keys.
Instead of this cmdlet, use Use-AadrmKeyVaultKey.
For more information, see Planning and implementing your Azure Rights Management tenant keyhttps://docs.microsoft.com/rights-management/plan-design/plan-implement-tenant-key (https://docs.microsoft.com/rights-management/plan-design/plan-implement-tenant-key) on the Microsoft documentation site.

## EXAMPLES

### Example 1: Add a tenant key
```
PS C:\> Add-AadrmKey -Force -KeyFile "C:\Keys\Key073"
```

This command adds the tenant key specified by the **KeyFile** parameter.
Because the command specifies the **Force** parameter, the command does not prompt you for confirmation.

## PARAMETERS

### -Force
Indicates that the cmdlet adds the tenant key silently without prompting you for confirmation.

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

### -KeyFile
Specifies a tenant key file packaged by using the tools to generate your tenant key over the Internet.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.Prompts you for confirmation before running the cmdlet.

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
The cmdlet is not run.Shows what would happen if the cmdlet runs.
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

## NOTES

## RELATED LINKS

[Use-AadrmKeyVaultKey](./Use-AadrmKeyVaultKey.md)

[Get-AadrmKeys](./Get-AadrmKeys.md)


