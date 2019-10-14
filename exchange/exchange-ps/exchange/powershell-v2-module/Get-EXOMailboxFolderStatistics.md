---
external help file: Microsoft.Exchange.Management.RestApiClient.dll-Help.xml
Module Name: ExchangeOnlineManagement
applicable: Exchange Online
title: Get-EXOMailboxFolderStatistics
schema: 2.0.0
author: chrisda
ms.author: chrisda
ms.reviewer:
monikerRange: "exchonline-ps"
---

# Get-EXOMailboxFolderStatistics

## SYNOPSIS
This cmdlet is available only in the Exchange Online PowerShell V2 module. For more information, see [Use the Exchange Online PowerShell V2 module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2).

Use the Get-EXOMailboxFolderStatistics cmdlet to retrieve information about the folders in a specified mailbox, including the number and size of items in the folder, the folder name and ID, and other information.

For information about the parameter sets in the Syntax section below, see Exchange cmdlet syntax (https://technet.microsoft.com/library/bb123552.aspx).

## SYNTAX

```
Get-EXOMailboxFolderStatistics
 [-Archive]
 [-ExternalDirectoryObjectId <Guid>]
 [-Folderscope <ElcFolderType>]
 [-Identity <String>]
 [-IncludeAnalysis]
 [-IncludeOldestAndNewestItems]
 [-IncludeSoftDeletedRecipients]
 [-ResultSize <Unlimited>]
 [-UserPrincipalName <String>]
 [<CommonParameters>]
```

## DESCRIPTION
A mailbox can have hidden items that are never visible to the user and are only used by applications. The Get-EXOMailboxFolderStatistics cmdlet can return hidden items for the following values: FolderSize, FolderAndSubfolderSize, ItemsInFolder and ItemsInFolderAndSubfolders.

The Get-EXOMailboxFolderStatistics cmdlet shouldn't be confused with the Get-EXOMailboxStatistics cmdlet.

## EXAMPLES

### Example 1
```
{{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -Archive
The Archive switch specifies whether to return the usage statistics of the archive associated with the mailbox or mail user. You don't need to specify a value with this switch.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:
Applicable: Exchange Online
Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExternalDirectoryObjectId
{{ Fill ExternalDirectoryObjectId Description }}

```yaml
Type: Guid
Parameter Sets: (All)
Aliases:
Applicable: Exchange Online
Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Folderscope
The FolderScope parameter specifies the scope of the search by folder type. Valid parameter values include:

- All

- Archive

- Calendar

- Clutter

- Contacts

- ConversationHistory

- DeletedItems

- Drafts

- Inbox

- Journal

- JunkEmail

- LegacyArchiveJournals

- ManagedCustomFolder

- NonIpmRoot

- Notes

- Outbox

- Personal

- RecoverableItems

- RssSubscriptions

- SentItems

- SyncIssues

- Tasks

```yaml
Type: ElcFolderType
Parameter Sets: (All)
Aliases:
Applicable: Exchange Online
Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Identity
The Identity parameter specifies the identity of the mailbox or mail user. You can use any value that uniquely identifies the mailbox or mail user. For example:

- Name

- Alias

- Distinguished name (DN)

- Canonical DN

- \<domain name\>\\\<account name\>

- Email address

- GUID

- LegacyExchangeDN

- SamAccountName

- User ID or user principal name (UPN)

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Applicable: Exchange Online
Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -IncludeAnalysis
The IncludeAnalysis switch specifies whether to scan all items within a folder and return statistics related to the folder and item size. You don't need to specify a value with this switch.

You should use this switch for troubleshooting purposes, because the command might take a long time to complete.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:
Applicable: Exchange Online
Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IncludeOldestAndNewestItems
The IncludeOldestAndNewestItems switch specifies whether to return the dates of the oldest and newest items in each folder. You don't need to specify a value with this switch.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:
Applicable: Exchange Online
Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -IncludeSoftDeletedRecipients
{{ Fill IncludeSoftDeletedRecipients Description }}

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:
Applicable: Exchange Online
Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResultSize
The ResultSize parameter specifies the maximum number of results to return. If you want to return all requests that match the query, use unlimited for the value of this parameter. The default value is 1000.

```yaml
Type: Unlimited
Parameter Sets: (All)
Aliases:
Applicable: Exchange Online
Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -UserPrincipalName
{{ Fill UserPrincipalName Description }}

```yaml
Type: String
Parameter Sets: (All)
Aliases:
Applicable: Exchange Online
Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (https://go.microsoft.com/fwlink/p/?LinkID=113216).

## INPUTS

###  

## OUTPUTS

###  

## NOTES

## RELATED LINKS

[Online Version](https://docs.microsoft.com/powershell/module/exchange/powershell-v2-module/get-exomailboxfolderstatistics)