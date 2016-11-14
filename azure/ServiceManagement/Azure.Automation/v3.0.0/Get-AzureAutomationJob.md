---
external help file: Microsoft.Azure.Commands.Automation.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: F200A4CD-58B4-499F-AAAB-03F31E03299C
updated_at: 11/11/2016 11:03 PM
ms.date: 11/11/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/live/azureps-cmdlets-docs/ServiceManagement/Azure.Automation/v3.0.0/Get-AzureAutomationJob.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/79eeb985ea480979357fb4695832a0c3d29a48bf/azureps-cmdlets-docs/ServiceManagement/Azure.Automation/v3.0.0/Get-AzureAutomationJob.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
id: ServiceManagement_Azure_Automation_v3_0_0_Get_AzureAutomationJob_md
---

# Get-AzureAutomationJob

## SYNOPSIS
Gets one or more Azure Automation runbook jobs.

## SYNTAX

### ByAll (Default)
```
Get-AzureAutomationJob [-Status <String>] [-StartTime <DateTimeOffset>] [-EndTime <DateTimeOffset>]
 [-AutomationAccountName] <String> [-Profile <AzureSMProfile>] [<CommonParameters>]
```

### ByJobId
```
Get-AzureAutomationJob -Id <Guid> [-AutomationAccountName] <String> [-Profile <AzureSMProfile>]
 [<CommonParameters>]
```

### ByRunbookName
```
Get-AzureAutomationJob -RunbookName <String> [-Status <String>] [-StartTime <DateTimeOffset>]
 [-EndTime <DateTimeOffset>] [-AutomationAccountName] <String> [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureAutomationJob** cmdlet gets one or more runbook jobs in Microsoft Azure Automation.

## EXAMPLES

### Example 1: Get a specific runbook job
```
PS C:\>Get-AzureAutomationJob -AutomationAccountName "Contoso17" -Id 2989b069-24fe-40b9-b3bd-cb7e5eac4b647
```

This command gets the job that has the specified GUID.

### Example 2: Get all jobs for a runbook
```
PS C:\>Get-AzureAutomationJob -AutomationAccountName "Contoso17" -RunbookName "MyRunbook"
```

This command gets all jobs associated with a runbook named MyRunbook.

### Example 2: Get all running jobs
```
PS C:\>Get-AzureAutomationJob -AutomationAccountName "Contoso17" -Status "Running"
```

This command gets all running jobs in the automation account with the name Contoso17.

## PARAMETERS

### -AutomationAccountName
Specifies the name of an Azure Automation account.

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

### -EndTime
Specifies the end time for a job.

```yaml
Type: DateTimeOffset
Parameter Sets: ByAll, ByRunbookName
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
Specifies the ID of a job.

```yaml
Type: Guid
Parameter Sets: ByJobId
Aliases: JobId

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -RunbookName
Specifies the name of a runbook.

```yaml
Type: String
Parameter Sets: ByRunbookName
Aliases: Name

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Status
Specifies the status of a job.
This cmdlet gets jobs that have a status matching this parameter.
Valid values are: 

- Completed
- Failed
- Queued
- Starting
- Resuming
- Running
- Stopped
- Stopping
- Suspended
- Suspending
- Activating

```yaml
Type: String
Parameter Sets: ByAll, ByRunbookName
Aliases: 
Accepted values: Completed, Failed, Queued, Starting, Resuming, Running, Stopped, Stopping, Suspended, Suspending, Activating, Blocked, Removing

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StartTime
Specifies the start time of a job.

```yaml
Type: DateTimeOffset
Parameter Sets: ByAll, ByRunbookName
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.Azure.Commands.Automation.Model.Job

## NOTES

## RELATED LINKS

[Resume-AzureAutomationJob](xref:ServiceManagement/Azure.Automation/v3.0.0/Resume-AzureAutomationJob.md)

[Stop-AzureAutomationJob](xref:ServiceManagement/Azure.Automation/v3.0.0/Stop-AzureAutomationJob.md)

[Suspend-AzureAutomationJob](xref:ServiceManagement/Azure.Automation/v3.0.0/Suspend-AzureAutomationJob.md)


