---
external help file: Microsoft.Open.AzureAD16.Graph.PowerShell.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 45C6B663-1AD4-4ED3-81BB-D2B79C67BC47
updated_at: 11/4/2016 6:14 PM
ms.date: 11/4/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-azuread/blob/master/Azure%20AD%20Cmdlets/AzureAD/v2/Get-AzureADApplicationOwner.md
gitcommit: https://github.com/Azure/azure-docs-powershell-azuread/blob/1307da5207c0612686b7bf1e036a30cf120993d3/Azure%20AD%20Cmdlets/AzureAD/v2/Get-AzureADApplicationOwner.md
ms.topic: reference
ms.prod: powershell
ms.service: Azure PowerShell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureADApplicationOwner

## SYNOPSIS
Gets the owner of an application.

## SYNTAX

```
Get-AzureADApplicationOwner -ObjectId <String> [-Top <Int32>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureADApplicationOwner** cmdlet get an owner of an Azure Active Directory application.

## EXAMPLES

### Example 1: Get the owner of an application
```PowerShell
PS C:\>Get-AzureADApplicationOwner -ObjectId "3ddd22e7-a150-4bb3-b100-e410dea1cb84"

ObjectId                             ObjectType
--------                             ----------
c13dd34a-492b-4561-b171-40fcce2916c5 User
```
This command gets the owner of an application.



## PARAMETERS

### -ObjectId
Specifes the ID of an application in Azure Active Directory.

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

### -Top
Specifies the maximum number of records to return.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
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
Specifies a variable in which to store an information event message.

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

[Add-AzureADApplicationOwner](xref:AzureAD/v2/Add-AzureADApplicationOwner.md)  
[Remove-AzureADApplicationOwner](xref:AzureAD/v2/Remove-AzureADApplicationOwner.md)

