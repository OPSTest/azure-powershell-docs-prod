---
external help file: Microsoft.Open.AzureAD16.Graph.PowerShell.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 8846536B-3E57-4307-81C7-CCFFB2C6E5EC
updated_at: 11/10/2016 7:26 PM
ms.date: 11/10/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2/Set-AzureADGroup.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/ae4f67ff36bc5b74558ace00c8475d6fc62f0c1f/Azure%20AD%20Cmdlets/AzureAD/v2/Set-AzureADGroup.md
ms.topic: reference
ms.prod: powershell
ms.service: active-directory
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Set-AzureADGroup

## SYNOPSIS
Updates a specific group in Azure Active Directory

## SYNTAX

```
Set-AzureADGroup -ObjectId <String> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [-Description <String>] [-DisplayName <String>] [-MailEnabled <Boolean>] [-MailNickName <String>]
 [-SecurityEnabled <Boolean>] [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureADGroup** cmdlet updates a group in Azure Active Directory (AD).

## EXAMPLES

### Example 1: Update a group
```PowerShell
PS C:\>Set-AzureADGroup -ObjectId "11fa5e1e-737c-40c5-835e-416ae3959606" -Description "This is my new group"
```
This command updates the specfied group in Azure AD.
## PARAMETERS

### -ObjectId
Specifies the object ID of a group.

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

### -Description
Specfies a description.
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

### -DisplayName
Specifies a display name.

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

### -MailEnabled
Indicates whether mail is enabled.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -MailNickName
Specifies a nickname for the mail.

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

### -SecurityEnabled
Indicates whether security is enabled.

```yaml
Type: Boolean
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

## NOTES

## RELATED LINKS
[Get-AzureADGroup](xref:AzureAD/v2/Get-AzureADGroup.md)

[New-AzureADGroup](xref:AzureAD/v2/New-AzureADGroup.md)

[Remove-AzureADGroup](xref:AzureAD/v2/Remove-AzureADGroup.md)
