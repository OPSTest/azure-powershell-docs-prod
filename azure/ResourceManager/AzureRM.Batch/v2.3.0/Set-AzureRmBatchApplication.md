---
external help file: Microsoft.Azure.Commands.Batch.dll-Help.xml
ms.assetid: 2475F266-C3FF-4AB0-87D6-6402EE2AC56B
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Batch/v2.3.0/Set-AzureRmBatchApplication.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.Batch/v2.3.0/Set-AzureRmBatchApplication.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Set-AzureRmBatchApplication

## SYNOPSIS
Updates settings for the specified application.

## SYNTAX

```
Set-AzureRmBatchApplication [-AccountName] <String> [-ResourceGroupName] <String> [-ApplicationId] <String>
 [[-DisplayName] <String>] [[-DefaultVersion] <String>] [[-AllowUpdates] <Boolean>] [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureRmBatchApplication** cmdlet modifies settings for the specified Azure Batch application.

## EXAMPLES

### Example 1: Update an application in a Batch account
```
PS C:\>Set-AzureRmBatchApplication -AccountName "ContosoBatch" -ResourceGroupName "ContosoBatchGroup" -ApplicationId "Litware" -AllowUpdates $False
```

This command changes whether the Llitware application in the ContosoBatch account allows updates.
The command does not change the default version or display name of the application.

## PARAMETERS

### -AccountName
Specifies the name of the Batch account for which this cmdlet modifies an application.

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

### -AllowUpdates
Specifies whether packages within the application can be overwritten using the same version string.

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases: 

Required: False
Position: 5
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ApplicationId
Specifies the ID of the application.

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

### -DefaultVersion
Specifies which package to use if a client requests the application but does not specify a version.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 4
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -DisplayName
Specifies the display name for the application.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group that contains the Batch account.

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

## NOTES

## RELATED LINKS

[Get-AzureRmBatchApplication](xref:ResourceManager/AzureRM.Batch/v2.3.0/Get-AzureRmBatchApplication.md)

[Get-AzureRmBatchApplicationPackage](xref:ResourceManager/AzureRM.Batch/v2.3.0/Get-AzureRmBatchApplicationPackage.md)

[New-AzureRmBatchApplication](xref:ResourceManager/AzureRM.Batch/v2.3.0/New-AzureRmBatchApplication.md)

[New-AzureRmBatchApplicationPackage](xref:ResourceManager/AzureRM.Batch/v2.3.0/New-AzureRmBatchApplicationPackage.md)

[Remove-AzureRmBatchApplication](xref:ResourceManager/AzureRM.Batch/v2.3.0/Remove-AzureRmBatchApplication.md)

[Remove-AzureRmBatchApplicationPackage](xref:ResourceManager/AzureRM.Batch/v2.3.0/Remove-AzureRmBatchApplicationPackage.md)

