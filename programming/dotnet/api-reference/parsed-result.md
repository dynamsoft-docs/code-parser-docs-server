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


```csharp
public class ParsedResult
```

## Methods

| Method               | Description |
|----------------------|-------------|
| [`GetOriginalImageHashId`](#getoriginalimagehashid) | Gets the hash ID of the source image. |
| [`GetOriginalImageTag`](#getoriginalimagetag) | Gets the tag of the source image. |
| [`GetItems`](#getitems) | Gets all the parsed result items. |
| [`GetErrorCode`](#geterrorcode) | Gets the error code of the parsed result, if an error occurred. |
| [`GetErrorString`](#geterrorstring) | Gets the error message of the parsed result, if an error occurred. |

### GetOriginalImageHashId

Gets the hash ID of the source image.

```csharp
string GetOriginalImageHashId()
```

**Return Value**

Returns a string containing the hash ID of the source image.

### GetOriginalImageTag

Gets the tag of the source image.

```csharp
ImageTag GetOriginalImageTag()
```

**Return Value**

Returns an `ImageTag` object representing the tag of the source image.

**See Also**

[ImageTag]({{ site.dcvb_dotnet_api }}core/basic-classes/image-tag.html)

### GetItems

Gets all the parsed result items.

```csharp
ParsedResultItem[] GetItems()
```

**Return Value**

Returns a `ParsedResultItem` array.

**See Also**

[ParsedResultItem]({{ site.dcp_dotnet_api }}parsed-result-item.html)

### GetErrorCode

Gets the error code of the parsed result, if an error occurred.

```csharp
int GetErrorCode()
```

**Return Value**

Returns the error code of the parsed result, or 0 if no error occurred.

**See Also**

[EnumErrorCode]({{ site.dcvb_dotnet_api }}core/enum-error-code.html)

### GetErrorString

Gets the error message of the parsed result, if an error occurred.

```csharp
string GetErrorString()
```

**Return Value**

Returns a string containing the error message of the parsed result, or an empty string if no error occurred.

