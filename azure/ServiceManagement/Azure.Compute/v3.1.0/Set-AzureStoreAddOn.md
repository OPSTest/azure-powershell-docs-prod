---
external help file: Microsoft.WindowsAzure.Commands.dll-Help.xml
ms.assetid: 7116CF7C-FFDC-4A1D-8D7E-AD70DE74BEEF
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v3.1.0/Set-AzureStoreAddOn.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v3.1.0/Set-AzureStoreAddOn.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: ServiceManagement_Azure_Compute_v3_1_0_Set_AzureStoreAddOn_md
---

# Set-AzureStoreAddOn

## SYNOPSIS
Updates an existing add-on instance.

## SYNTAX

```
Set-AzureStoreAddOn [-Name] <String> [-Plan] <String> [[-PromotionCode] <String>] [-PassThru]
 [-Profile <AzureSMProfile>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [<CommonParameters>]
```

## DESCRIPTION
This topic describes the cmdlet in the 0.8.10 version of the Microsoft Azure PowerShell module.
To get the version of the module you're using, in the Azure PowerShell console, type (Get-Module -Name Azure).Version.

This cmdlet updates an existing add-on instance from the current subscription.

## EXAMPLES

### Example 1
```
PS C:\>Set-AzureStoreAddOn MyAddOn NewPlanId
```

This example updates an add-on with a new plan ID.

### Example 2
```
PS C:\>Set-AzureStoreAddOn MyAddOn NewPlanId MyPromoCode
```

This example updates an add-on with a new plan ID and promotional code.

## PARAMETERS

### -Name
Specifies the name of the add-on instance.

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

### -Plan
Specifies the plan ID.

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

### -PromotionCode
Specifies the promotional code.

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

### -PassThru
If specified, the cmdlet returns true if the command succeeds and false if it fails.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
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

[Get-AzureStoreAddOn](xref:ServiceManagement/Azure.Compute/v3.1.0/Get-AzureStoreAddOn.md)

[New-AzureStoreAddOn](xref:ServiceManagement/Azure.Compute/v3.1.0/New-AzureStoreAddOn.md)

[Remove-AzureStoreAddOn](xref:ServiceManagement/Azure.Compute/v3.1.0/Remove-AzureStoreAddOn.md)


