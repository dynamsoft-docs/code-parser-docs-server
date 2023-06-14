---
layout: default-layout
title: CParsedResultItem Class - Dynamsoft Code Parser SDK C++ Edition API Reference
description: This page shows CParsedResultItem Class of Dynamsoft Code Parser SDK C++ Edition.
keywords: CParsedResultItem, api reference, c++
needAutoGenerateSidebar: true
---


# CParsedResultItem Class

```cpp
class dynamsoft::dcp::CParsedResultItem
```

  | Method               | Description |
  |----------------------|-------------|
  | [`GetCodeType`](#getcodetype) | Get all recognized barcode results. |
  | [`GetFieldMappingStatus`](#getfieldmappingstatus) | Get intermediate results. |
  | [`GetFieldValidationStatus`](#getfieldvalidationstatus) | Free memory allocated for the intermediate results. |
  | [`GetFieldValue`](#getfieldvalue) | Free memory allocated for text results. |
  | [`GetJsonString`](#getjsonstring) | Get all recognized barcode results. |
  
## GetCodeType

Gets the code type of the parsed result.

```cpp
const char* dynamsoft::dcp::CParsedResultItem::GetCodeType()
```

**Return Value**

Returns a string value representing the code type.

## GetJsonString

Gets the parsed result as a JSON formatted string.

```cpp
const char* dynamsoft::dcp::CParsedResultItem::GetJsonString()
```

**Return Value**

Returns a JSON formatted string representing the parsed result.

## GetFieldValue

Gets the value of a specified field from the parsed result.

```cpp
const char* dynamsoft::dcp::CParsedResultItem::GetFieldValue (const char* fieldName)
```

**Parameters**

`[in] fieldName` The name of the field.

**Return Value**

Returns a string representing the specified field value.

## GetFieldMappingStatus

Gets the mapping status of a specified field from the parsed result.

```cpp
MappingStatus dynamsoft::dcp::CParsedResultItem::GetFieldMappingStatus(const char* fieldName)
```

**Parameters**

`[in] fieldName` The name of the field.


**Return Value**

Returns a [MappingStatus]({{site.cpp_enum}}mapping-status.html) representing the mapping status of a specified field.

**See Also**

[MappingStatus]({{site.cpp_enum}}mapping-status.html)

## GetFieldValidationStatus

Gets the validation status of a specified field from the parsed result.

```cpp
ValidationStatus dynamsoft::dcp::CParsedResultItem::GetFieldValidationStatus(const char* fieldName)
```

**Parameters**

`[in] fieldName` The name of the field.

**Return Value**

Returns a [ValidationStatus]({{site.cpp_enum}}validation-status.html) representing the validation status of a specified field.

**See Also**

[ValidationStatus]({{site.cpp_enum}}validation-status.html)
