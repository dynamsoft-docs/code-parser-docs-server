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
  | [`GetCodeType`](#getcodetype) | Gets the code type of the parsed result. |
  | [`GetFieldMappingStatus`](#getfieldmappingstatus) | Gets the mapping status of a specified field from the parsed result. |
  | [`GetFieldValidationStatus`](#getfieldvalidationstatus) | Gets the validation status of a specified field from the parsed result. |
  | [`GetFieldRawValue`](#getfieldrawvalue) | Gets the raw string of a specified field from the parsed result. |
  | [`GetFieldValue`](#getfieldvalue) | Gets the value of a specified field from the parsed result. |
  | [`GetJsonString`](#getjsonstring) | Gets the parsed result as a JSON formatted string. |
  | [`GetFieldCount`](#getfieldcount) | Gets the total number of parsed fields. |
  | [`GetFieldName`](#getfieldname) | Gets the name of a specific parsed field by its index. |

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

## GetFieldRawValue

Gets the raw string of a specified field from the parsed result.

```cpp
const char* GetFieldRawValue(const char* fieldName)
```

**Parameters**

`[in] fieldName` The name of the field.

**Return Value**

Returns a string representing the specified field raw string.

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

Returns a [MappingStatus]({{ site.dcvb_cpp_api }}enum-mapping-status.html?lang=cpp) enumeration value representing the mapping status of a specified field.

**See Also**

[MappingStatus]({{ site.dcvb_cpp_api }}enum-mapping-status.html?lang=cpp)

## GetFieldValidationStatus

Gets the validation status of a specified field from the parsed result.

```cpp
ValidationStatus dynamsoft::dcp::CParsedResultItem::GetFieldValidationStatus(const char* fieldName)
```

**Parameters**

`[in] fieldName` The name of the field.

**Return Value**

Returns a [ValidationStatus]({{ site.dcvb_cpp_api }}enum-validation-status.html?lang=cpp) enumeration value representing the validation status of a specified field.

**See Also**

[ValidationStatus]({{ site.dcvb_cpp_api }}enum-validation-status.html?lang=cpp)

## GetFieldCount

Gets the total number of parsed fields.

```cpp
int GetFieldCount()
```

**Return Value**

Returns an integer representing the count of parsed fields.

## GetFieldName

Gets the name of a specific parsed field by its index.

```cpp
const char* GetFieldName(const int index)
```

**Parameters**

`[in] index` The index of the parsed field.

**Return Value**

Returns a string representing the specified field name.

If the field is nested, the name includes all parent fields, separated by a dot (.). The format follows this pattern: <root_field>[.<child_field1>[.<child_field2>...]]
