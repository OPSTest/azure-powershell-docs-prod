---
external help file: Microsoft.Azure.Commands.OperationalInsights.dll-Help.xml
online version: 3a46bcd5-ad81-411a-92aa-7788ebd2473e
schema: 2.0.0
ms.assetid: 3314D7A0-A0DB-418B-A0C9-8455819C65AA
updated_at: 10/24/2016 11:18 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.OperationalInsights/v2.2.0/Get-AzureRmOperationalInsightsStorageInsight.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/7db57df6b5e709a7c001e6de362a1240d7583ae8/azureps-cmdlets-docs/ResourceManager/AzureRM.OperationalInsights/v2.2.0/Get-AzureRmOperationalInsightsStorageInsight.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureRmOperationalInsightsStorageInsight

## SYNOPSIS
Gets information about a Storage Insight.

## SYNTAX

### ByWorkspaceName (Default)
```
Get-AzureRmOperationalInsightsStorageInsight [-ResourceGroupName] <String> [-WorkspaceName] <String>
 [[-Name] <String>] [<CommonParameters>]
```

### ByWorkspaceObject
```
Get-AzureRmOperationalInsightsStorageInsight [-Workspace] <PSWorkspace> [[-Name] <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmOperationalInsightsStorageInsight** cmdlet gets information about an existing Storage Insight.
If a Storage Insight name is specified, this cmdlet gets information about that Storage Insight.
If you do not specify a name, this cmdlet gets information about all storage insights in a workspace.

## EXAMPLES

### Example 1: Get a Storage Insight by name
```
PS C:\>Get-AzureRmOperationalInsightsStorageInsight  ¢â‚¬"Name "MyStorageInsight"  ¢â‚¬"ResourceGroupName "ContosoResourceGroup"  ¢â‚¬"WorkspaceName "ContosoWorkspace"
```

This command gets the storage insight named MyStorageInsight from the workspace named ContosoWorkspace.

### Example 2: Get a Storage Insight by using a workspace object
```
PS C:\>$Workspace = Get-AzureRmOperationalInsightsWorkspace  ¢â‚¬"ResourceGroupName "ContosoResourceGroup"  ¢â‚¬"Name "MyWorkspace"
PS C:\>Get-AzureRmOperationalInsightsStorageInsight  ¢â‚¬"Workspace $Workspace  ¢â‚¬"Name "MyStorageInsight"
```

The first command uses the **Get-AzureRmOperationalInsightsWorkspace** cmdlet to get an Operational Insights workspace, and then stores it in the $Workspace variable.

The second command gets the storage insight named MyStorageInsight for the workspace in $Workspace.

## PARAMETERS

### -ResourceGroupName
Specifies the name of an Azure resource group.

```yaml
Type: String
Parameter Sets: ByWorkspaceName
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -WorkspaceName
Specifies the name of the workspace that contains the Storage Insights.

```yaml
Type: String
Parameter Sets: ByWorkspaceName
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the Storage Insight name.

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

### -Workspace
Specifies the workspace that contains the Storage Insights.

```yaml
Type: PSWorkspace
Parameter Sets: ByWorkspaceObject
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

[Azure Operational Insights Cmdlets](.\AzureRM.OperationalInsights.md)

