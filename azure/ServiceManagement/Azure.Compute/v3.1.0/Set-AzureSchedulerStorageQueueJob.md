---
external help file: Microsoft.WindowsAzure.Commands.dll-Help.xml
ms.assetid: A8E69695-F5A6-4F37-A743-8F89C9972167
online version: 
schema: 2.0.0
updated_at: 11/8/2016 12:38 AM
ms.date: 11/8/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v3.1.0/Set-AzureSchedulerStorageQueueJob.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/04b9ae2d1c44a3ada330f570237886794cede893/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v3.1.0/Set-AzureSchedulerStorageQueueJob.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
ms.author: PowerShellHelpPub
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Set-AzureSchedulerStorageQueueJob

## SYNOPSIS
Updates a scheduler job that has a storage action.

## SYNTAX

### Required
```
Set-AzureSchedulerStorageQueueJob [-Location] <String> [-JobCollectionName] <String> [-JobName] <String>
 [[-StorageQueueAccount] <String>] [[-StorageQueueName] <String>] [[-SASToken] <String>]
 [[-StorageQueueMessage] <String>] [[-StartTime] <DateTime>] [[-Interval] <Int32>] [[-Frequency] <String>]
 [[-EndTime] <DateTime>] [[-ExecutionCount] <Int32>] [[-JobState] <String>] [[-ErrorActionMethod] <String>]
 [[-ErrorActionURI] <Uri>] [[-ErrorActionRequestBody] <String>] [[-ErrorActionHeaders] <Hashtable>]
 [[-ErrorActionStorageAccount] <String>] [[-ErrorActionStorageQueue] <String>]
 [[-ErrorActionSASToken] <String>] [[-ErrorActionQueueMessageBody] <String>] [-PassThru]
 [-Profile <AzureSMProfile>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [<CommonParameters>]
```

### Recurring
```
Set-AzureSchedulerStorageQueueJob [[-Interval] <Int32>] [[-Frequency] <String>] [[-EndTime] <DateTime>]
 [[-ExecutionCount] <Int32>] [[-JobState] <String>] [[-ErrorActionHeaders] <Hashtable>] [-PassThru]
 [-Profile <AzureSMProfile>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [<CommonParameters>]
```

## DESCRIPTION
This topic describes the cmdlet in the 0.8.10 version of the Microsoft Azure PowerShell module.
To get the version of the module you're using, in the Azure PowerShell console, type (Get-Module -Name Azure).Version.

The **Set-AzureSchedulerStorageQueueJob** cmdlet updates a scheduler job that has an Azure Storage action.

## EXAMPLES

### Example 1: Update a Storage queue message
```
PS C:\>Set-AzureSchedulerStorageQueueJob -Location "North Central US" -JobCollectionName "JobCollection01 -JobName "Job12" -StorageQueueMessage "Updated message"
```

This command updates the queue message for the Storage job named Job12.
The command specifies the job collection name and the location.

### Example 2: Enable a Storage queue job
```
PS C:\>Set-AzureSchedulerStorageQueueJob -Location "North Central US" -JobCollectionName "JobCollection02" -JobName "Job16" -JobState "Enabled"
```

This command enables the job named Job16.
The command changes the state of the job to Enabled by specifying that value for the *JobState* parameter.

## PARAMETERS

### -Location
Specifies the name of the location that hosts the cloud service.
Valid values are: 

- Anywhere Asia
- Anywhere Europe
- Anywhere US
- East Asia
- East US
- North Central US
- North Europe
- South Central US
- Southeast Asia
- West Europe
- West US

```yaml
Type: String
Parameter Sets: Required
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -JobCollectionName
Specifies the name of the collection to contain the scheduler job.

```yaml
Type: String
Parameter Sets: Required
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -JobName
Specifies the name of the scheduler job to update.

```yaml
Type: String
Parameter Sets: Required
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -StorageQueueAccount
Specifies the Storage account name.

```yaml
Type: String
Parameter Sets: Required
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -StorageQueueName
Specifies the name of the Storage queue.

```yaml
Type: String
Parameter Sets: Required
Aliases: 

Required: False
Position: 4
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -SASToken
Specifies the SAS token for the Storage queue.

```yaml
Type: String
Parameter Sets: Required
Aliases: 

Required: False
Position: 5
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -StorageQueueMessage
Specifies the queue message for the Storage job.

```yaml
Type: String
Parameter Sets: Required
Aliases: 

Required: False
Position: 6
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StartTime
Specifies a time, as a **DateTime** object, for the job to start.

```yaml
Type: DateTime
Parameter Sets: Required
Aliases: 

Required: False
Position: 8
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Interval
Specifies the interval of recurrence at the frequency specified by using the *Frequency* parameter.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: 9
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Frequency
Specifies the maximum frequency for this scheduler job.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 10
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -EndTime
Specifies a time, as a **DateTime** object, for the scheduler to stop initiating the job.
To obtain a **DateTime** object, use the **Get-Date** cmdlet.
For more information, type `Get-Help Get-Date`.

```yaml
Type: DateTime
Parameter Sets: (All)
Aliases: 

Required: False
Position: 11
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExecutionCount
Specifies the number occurrences of a job that run.
By default, a job recurs indefinitely.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: 12
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -JobState
Specifies the state for the scheduler job.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 13
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ErrorActionMethod
Specifies the method for HTTP and HTTPS action types.
Valid values are: 

- GET
- PUT
- POST
- HEAD
- DELETE

```yaml
Type: String
Parameter Sets: Required
Aliases: 

Required: False
Position: 14
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ErrorActionURI
Specifies the URI for the error job action.

```yaml
Type: Uri
Parameter Sets: Required
Aliases: 

Required: False
Position: 15
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ErrorActionRequestBody
Specifies the body for PUT and POST job actions.

```yaml
Type: String
Parameter Sets: Required
Aliases: 

Required: False
Position: 16
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ErrorActionHeaders
Specifies headers as a hash table.

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases: 

Required: False
Position: 17
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ErrorActionStorageAccount
Specifies the name of the Storage account.

```yaml
Type: String
Parameter Sets: Required
Aliases: 

Required: False
Position: 18
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ErrorActionStorageQueue
Specifies the name of the Storage queue.

```yaml
Type: String
Parameter Sets: Required
Aliases: 

Required: False
Position: 19
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ErrorActionSASToken
Specifies the Shared Access Signature (SAS) token for the Storage queue.

```yaml
Type: String
Parameter Sets: Required
Aliases: 

Required: False
Position: 20
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ErrorActionQueueMessageBody
Specifies the body for Storage job actions.

```yaml
Type: String
Parameter Sets: Required
Aliases: 

Required: False
Position: 21
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
Indicates that this cmdlet returns an object representing the item on which it operates.
By default, this cmdlet does not generate any output.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
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

[New-AzureSchedulerStorageQueueJob](xref:ServiceManagement/Azure.Compute/v3.1.0/New-AzureSchedulerStorageQueueJob.md)

