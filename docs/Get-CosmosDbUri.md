---
external help file: CosmosDB-help.xml
Module Name: CosmosDB
online version:
schema: 2.0.0
---

# Get-CosmosDbUri

## SYNOPSIS

Return the URI of the CosmosDB that Rest APIs requests will
be sent to.

## SYNTAX

```powershell
Get-CosmosDbUri [-Account] <String> [[-BaseUri] <String>] [<CommonParameters>]
```

## DESCRIPTION

This cmdlet returns the root URI of the CosmosDB.

## EXAMPLES

### EXAMPLE 1

```powershell
PS C:\> $uri = Get-CosmosDbUri -Account 'MyAzureCosmosDB'
```

Generates the URI for accessing an Azure CosmosDB account.

### EXAMPLE 2

```powershell
PS C:\>$uri = Get-CosmosDbUri -Account 'MyAzureCosmosDB' -BaseUri 'localhost'
```

Generates the URI for accessing a CosmosDB emulator account
on the localhost.

## PARAMETERS

### -Account

This is the name of the CosmosDB Account to get the URI
for.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BaseUri

This is the base URI of the CosmosDB to use.
If not specified it will default to 'documents.azure.com'.

```yaml
Type: String
Parameter Sets: (All)
Aliases:

Required: False
Position: 2
Default value: Documents.azure.com
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters

This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable.
For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### System.Uri

## NOTES

## RELATED LINKS
