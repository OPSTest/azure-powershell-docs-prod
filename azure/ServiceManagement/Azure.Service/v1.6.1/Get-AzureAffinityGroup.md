---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 985D040B-1148-40B1-ACDD-8C30DD3C7B29
updated_at: 11/1/2016 10:24 PM
ms.date: 11/1/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v1.6.1/Get-AzureAffinityGroup.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/f59f3ef60bc592383812213e69fd77ba950759ed/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v1.6.1/Get-AzureAffinityGroup.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: ServiceManagement_Azure_Service_v1_6_1_Get_AzureAffinityGroup_md
---

# Get-AzureAffinityGroup

## SYNOPSIS
Gets an Azure affinity group object.

## SYNTAX

```
Get-AzureAffinityGroup [[-Name] <String>] [-Profile <AzureSMProfile>] [-InformationAction <ActionPreference>]
 [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureAffinityGroup** cmdlet gets an Azure affinity group.
The affinity group object includes the affinity group name, location, label, description and the storage and hosted services that are part of the affinity group.

## EXAMPLES

### Example 1: Get properties of an affinity group
```
PS C:\>Get-AzureAffinityGroup -Name "South01"
```

This command gets the properties of the affinity group named South01.

## PARAMETERS

### -Name
Specifies the name of the affinity group that this cmdlet gets.
Names for affinity groups created through the Management Portal are typically GUIDs.
The Management Port shows the affinity group label.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Profile
ps_azureprofile_description

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

### AffinityGroup

## NOTES

## RELATED LINKS

[New-AzureAffinityGroup](xref:ServiceManagement/Azure.Service/v1.6.1/New-AzureAffinityGroup.md)

[Remove-AzureAffinityGroup](xref:ServiceManagement/Azure.Service/v1.6.1/Remove-AzureAffinityGroup.md)

[Set-AzureAffinityGroup](xref:ServiceManagement/Azure.Service/v1.6.1/Set-AzureAffinityGroup.md)


