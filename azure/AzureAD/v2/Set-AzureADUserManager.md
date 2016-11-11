---
external help file: Microsoft.Open.AzureAD16.Graph.PowerShell.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: B218B2D5-04BF-4957-9902-1DBE75C746E4
updated_at: 11/7/2016 10:54 PM
ms.date: 11/7/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2/Set-AzureADUserManager.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/5e545bcc775e42a595163d0e9dd005852457a8f8/Azure%20AD%20Cmdlets/AzureAD/v2/Set-AzureADUserManager.md
ms.topic: reference
ms.prod: 
ms.service: active-directory
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: AzureAD_v2_Set_AzureADUserManager_md
---

# Set-AzureADUserManager

## SYNOPSIS
Updates a user's manager.

## SYNTAX

```
Set-AzureADUserManager -ObjectId <String> -RefObjectId <String> [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureADUserManager** cmdlet update the manager for a user in Azure Active Directory (AD).
## EXAMPLES

### Example 1: Update a user's manager
```PowerShell
PS C:\>Set-AzureADUserManager -ObjectId "df19e8e6-2ad7-453e-87f5-037f6529ae16" -RefObjectId "df19e8e6-2ad7-453e-87f5-037f6529ae16"
```
This command update's the manager for the specified user.
## PARAMETERS

### -ObjectId
Specifies the ID (as a UPN or ObjectId) of a user in Azure AD. 

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

### -RefObjectId
Specifies the ID of the Azure AD object to assign as owner/manager/member.

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

### -InformationAction
Specifies how this cmdlet responds to an information event. The acceptable values for this parameter are:

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
[Get-AzureADUserManager](xref:AzureAD/v2/Get-AzureADUserManager.md)

[Remove-AzureADUserManager](xref:AzureAD/v2/Remove-AzureADUserManager.md)

