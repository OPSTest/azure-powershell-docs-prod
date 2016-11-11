---
external help file: Microsoft.Azure.Commands.Websites.dll-Help.xml
ms.assetid: 01D98F26-A631-4E25-97AE-92D0B1355E0E
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ResourceManager/AzureRM.Websites/v2.3.0/Set-AzureRmAppServicePlan.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ResourceManager/AzureRM.Websites/v2.3.0/Set-AzureRmAppServicePlan.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Set-AzureRmAppServicePlan

## SYNOPSIS
Sets an Azure App Service plan.

## SYNTAX

### S1
```
Set-AzureRmAppServicePlan [[-AdminSiteName] <String>] [[-Tier] <String>] [[-NumberofWorkers] <Int32>]
 [[-WorkerSize] <String>] [-ResourceGroupName] <String> [-Name] <String> [<CommonParameters>]
```

### S2
```
Set-AzureRmAppServicePlan [-AppServicePlan] <ServerFarmWithRichSku> [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureRmAppServicePlan** cmdlet sets an Azure App Service plan.

## EXAMPLES

### 1:
```

```

## PARAMETERS

### -AdminSiteName
```yaml
Type: String
Parameter Sets: S1
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Tier
```yaml
Type: String
Parameter Sets: S1
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NumberofWorkers
```yaml
Type: Int32
Parameter Sets: S1
Aliases: 

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WorkerSize
```yaml
Type: String
Parameter Sets: S1
Aliases: 

Required: False
Position: 5
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
```yaml
Type: String
Parameter Sets: S1
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
```yaml
Type: String
Parameter Sets: S1
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AppServicePlan
```yaml
Type: ServerFarmWithRichSku
Parameter Sets: S2
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmWebApp](xref:ResourceManager/AzureRM.Websites/v2.3.0/Get-AzureRmWebApp.md)

[New-AzureRmWebApp](xref:ResourceManager/AzureRM.Websites/v2.3.0/New-AzureRmWebApp.md)

[Remove-AzureRmWebApp](xref:ResourceManager/AzureRM.Websites/v2.3.0/Remove-AzureRmWebApp.md)

[Restart-AzureRmWebApp](xref:ResourceManager/AzureRM.Websites/v2.3.0/Restart-AzureRmWebApp.md)

[Start-AzureRmWebApp](xref:ResourceManager/AzureRM.Websites/v2.3.0/Start-AzureRmWebApp.md)

[Stop-AzureRmWebApp](xref:ResourceManager/AzureRM.Websites/v2.3.0/Stop-AzureRmWebApp.md)


