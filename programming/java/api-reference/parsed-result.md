---
layout: default-layout
title: ParsedResult Class - Dynamsoft Code Parser Module Java Edition API Reference
description: Definition of the ParsedResult class in Dynamsoft Code Parser Module Java Edition.
keywords: ParsedResult, api reference, java
---

# ParsedResult Class

The `ParsedResult` class represents the results of a code parser process.

## Definition

*Package:* com.dynamsoft.dcp

```java
public class ParsedResult extends CapturedResultBase
```

## Methods

| Method               | Description |
|----------------------|-------------|
| [`getItemsCount`](#getitemscount) | Gets the count of parsed result items. |
| [`getItem`](#getitem) | Gets a parsed result item at the specified index. |
| [`getItems`](#getitems) | Gets all the parsed result items. |

### getItemsCount

Gets the count of parsed result items.

```java
public int getItemsCount()
```

**Return Value**

Returns the number of parsed result items.

### getItem

Gets a parsed result item at the specified index.

```java
public ParsedResultItem getItem(int index)
```

**Parameters**

`index` The index of the parsed result item.

**Return Value**

Returns a `ParsedResultItem` object at the specified index.

**See Also**

[ParsedResultItem]({{ site.dcp_java_api }}parsed-result-item.html)

### getItems

Gets all the parsed result items.

```java
public ParsedResultItem[] getItems()
```

**Return Value**

Returns an array of `ParsedResultItem` objects.

**See Also**

[ParsedResultItem]({{ site.dcp_java_api }}parsed-result-item.html)

