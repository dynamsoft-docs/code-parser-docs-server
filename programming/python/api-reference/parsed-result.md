---
layout: default-layout
title: ParsedResult Class - Dynamsoft Code Parser Module Python Edition API Reference
description: Definition of the ParsedResult class in Dynamsoft Code Parser Module Python Edition.
keywords: ParsedResult, api reference, python
needAutoGenerateSidebar: true
---

# ParsedResult Class

The `ParsedResult` class represents the results of a code parser process.

## Definition

*Module:* dynamsoft_code_parser

```python
class ParsedResult
```

## Methods

| Method               | Description |
|----------------------|-------------|
| [`get_original_image_hash_id`](#get_original_image_hash_id) | Gets the hash ID of the source image. |
| [`get_original_image_tag`](#get_original_image_tag) | Gets the tag of the source image. |
| [`get_items`](#get_items) | Gets all the parsed result items. |
| [`get_error_code`](#get_error_code) | Gets the error code of the parsed result, if an error occurred. |
| [`get_error_string`](#get_error_string) | Gets the error message of the parsed result, if an error occurred. |

### get_original_image_hash_id

Gets the hash ID of the source image.

```python
def get_original_image_hash_id(self) -> str:
```

**Return Value**

Returns a string containing the hash ID of the source image.

### get_original_image_tag

Gets the tag of the source image.

```python
def get_original_image_tag(self) -> ImageTag:
```

**Return Value**

Returns an `ImageTag` object representing the tag of the source image.

**See Also**

[ImageTag]({{ site.dcvb_python_api }}core/basic-classes/image-tag.html)

### get_items

Gets all the parsed result items.

```python
def get_items(self) -> List[ParsedResultItem]:
```

**Return Value**

Returns a `ParsedResultItem` list.

**See Also**

[ParsedResultItem]({{ site.dcp_python_api }}parsed-result-item.html)

### get_error_code

Gets the error code of the parsed result, if an error occurred.

```python
def get_error_code(self) -> int:
```

**Return Value**

Returns the error code of the parsed result, or 0 if no error occurred.

**See Also**

[EnumErrorCode]({{ site.dcvb_python_api }}core/enum-error-code.html?lang=python)

### get_error_string

Gets the error message of the parsed result, if an error occurred.

```python
def get_error_string(self) -> str:
```

**Return Value**

Returns a string containing the error message of the parsed result, or an empty string if no error occurred.

