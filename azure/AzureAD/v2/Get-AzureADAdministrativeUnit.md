---
external help file: azuread.help.xml
online version: https://blogs.technet.microsoft.com/enterprisemobility/2016/07/18/azuread-certificate-based-authentication-for-ios-and-android-now-in-preview/
schema: 2.0.0
updated_at: 11/21/2016 8:09 PM
ms.date: 11/21/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2/Get-AzureADAdministrativeUnit.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/e79870303c4a5b18f88c61a5fe206bd45af8c480/Azure%20AD%20Cmdlets/AzureAD/v2/Get-AzureADAdministrativeUnit.md
ms.topic: reference
ms.prod: 
ms.service: active-directory
ms.technology: Azure PowerShell
author: erickson-doug
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: carolz
id: AzureAD_v2_Get_AzureADAdministrativeUnit_md
---

# Get-AzureADAdministrativeUnit

## SYNOPSIS
Get an Administrative Unit by objectId

## SYNTAX

### UNNAMED_PARAMETER_SET_1
```
Get-AzureADAdministrativeUnit -ObjectId <String>
```

### UNNAMED_PARAMETER_SET_2
```
Get-AzureADAdministrativeUnit [-Top <Int32>] [-Filter <String>]
```

## DESCRIPTION

## EXAMPLES

### Example 1
```

```

## PARAMETERS

### -ObjectId
The unique idenfier of an administrativeUnit in Azure Active Directory

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_1
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Top
The maximum number of records to return.
If no value is provided, 100 records are returned

```yaml
Type: Int32
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Filter
The oData v3.0 filter statement. 
Controls which objects are returned.

To learn more about oData v3.0 filter expressions, refer to https://msdn.microsoft.com/en-us/library/hh169248%28v=nav.90%29.aspx

```yaml
Type: String
Parameter Sets: UNNAMED_PARAMETER_SET_2
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES
Please note that this cmdlet is currently in Public Preview.
While a cmdlet is in Public Preview we may still need to make changes to the cmdlet which could potentially cause unexpected effects.
We discourage customers from using this cmdlet in a production environment.

## RELATED LINKS

