---
external help file: Microsoft.Azure.Commands.ManagedCache.dll-Help.xml
ms.assetid: 0C78C20D-DE00-4923-95E7-0EE619CF645B
online version: 
schema: 2.0.0
---

# Get-AzureManagedCacheAccessKey

## SYNOPSIS
Gets the access keys for an Azure Cache.

## SYNTAX

```
Get-AzureManagedCacheAccessKey [-Name] <String> [-Profile <AzureSMProfile>]
 [-InformationAction <ActionPreference>] [-InformationVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureManagedCacheAccessKey** cmdlet gets the primary and secondary access keys for an Azure Cache.
You can use these keys to allow clients, such as web applications, to access to your Azure Cache.
Typically, you use the primary key, but use the secondary key to avoid delays while the primary key is being regenerated.
To get new access keys, use the New-AzureManagedCacheAccessKey cmdlet.
An Azure Cache is a secure, dedicated cache that provides extremely fast access to data.
This distributed, in-memory, scalable solution enables you to build highly scalable and responsive applications.
For more information about Azure Cache, see [Azure Cache](http://azure.microsoft.com/en-us/services/cache/) (http://azure.microsoft.com/en-us/services/cache/).

## EXAMPLES

### Example 1: Get the access key for an Azure Cache
```
PS C:\>Get-AzureManagedCacheAccessKey -Name "ContosoCache"
```

This command gets the access key for the Azure Cache named ContosoCache.

## PARAMETERS

### -Name
Specifies the name of the Azure Cache.
This parameter value is case-sensitive.
Wildcard characters are not permitted.

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

### None

## OUTPUTS

### Microsoft.Azure.Management.ManagedCache.Models.CachingKeysResponse

## NOTES

## RELATED LINKS

[New-AzureManagedCacheAccessKey](./New-AzureManagedCacheAccessKey.md)

[New-AzureManagedCache](./New-AzureManagedCache.md)

[Get-AzureManagedCache](./Get-AzureManagedCache.md)

[Set-AzureManagedCache](./Set-AzureManagedCache.md)

[Remove-AzureManagedCache](./Remove-AzureManagedCache.md)


