---
layout: default-layout
title: ParsedResult Class - Dynamsoft Code Parser Module .NET Edition API Reference
description: Definition of the ParsedResult class in Dynamsoft Code Parser Module .NET Edition.
keywords: ParsedResult, api reference, .NET
needAutoGenerateSidebar: true
---

# ParsedResult Class

The `ParsedResult` class represents the results of a code parser process.

## Definition

*Namespace:* Dynamsoft.DCP

*Inheritance:* [CapturedResultBase]({{ site.dcvb_dotnet_api }}core/basic-classes/captured-result-base.html) -> ParsedResult

```csharp
public class ParsedResult : CapturedResultBase, IEnumerable<ParsedResultItem>
```

## Methods

| Method               | Description |
|----------------------|-------------|
| [`GetItemsCount`](#getitemscount)           | Gets the number of parsed result items.|
| [`GetItem`](#getitem)           | Gets a `ParsedResultItem` object at the specified index.|
| [`GetItems`](#getitems) | Gets all the parsed result items. |

### GetItemsCount

Gets the number of parsed result items.

```csharp
int GetItemsCount()
```

**Return value**

Returns the number of parsed result items.

### GetItem

Gets a `ParsedResultItem` object at the specified index.

```csharp
ParsedResultItem GetItem(int index)
```

**Parameter**

`[in] index` The index of the desired `ParsedResultItem` object.

**Return value**

Returns the `ParsedResultItem` object at the specified index.

**See Also**

[ParsedResultItem]({{ site.dbr_dotnet_api }}parsed-result-item.html)


### GetItems

Gets all the parsed result items.

```csharp
ParsedResultItem[] GetItems()
```

**Return Value**

Returns a `ParsedResultItem` array.

**See Also**

[ParsedResultItem]({{ site.dcp_dotnet_api }}parsed-result-item.html)

