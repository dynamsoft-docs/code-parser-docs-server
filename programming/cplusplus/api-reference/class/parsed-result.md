---
layout: default-layout
title: CParsedResult Class - Dynamsoft Code Parser SDK C++ Edition API Reference
description: This page shows CParsedResult Class of Dynamsoft Code Parser SDK C++ Edition.
keywords: CParsedResult, api reference, c++
needAutoGenerateSidebar: true
permalink: /programming/cplusplus/api-reference/parsed-result.html
---


# CParsedResult Class

```cpp
class dynamsoft::dcp::CParsedResult
```

| Method               | Description |
|----------------------|-------------|
| [`GetSourceImageHashId`](#getsourceimagehashid) | Gets the hash ID of the source image. |
| [`GetSourceImageTag`](#getsourceimagetag) | Gets the tag of the source image. |
| [`GetCount`](#getcount) | Gets the number of parsed result items in the parsed result. |
| [`GetItem`](#getitem) | Gets the parsed result item at the specified index. |
| [`GetErrorCode`](#geterrorcode) | Gets the error code of the parsed result, if an error occurred. |
| [`GetErrorString`](#geterrorstring) | Gets the error message of the parsed result, if an error occurred. |

### GetSourceImageHashId

Gets the hash ID of the source image.

```cpp
virtual const char* GetSourceImageHashId() const = 0;
```

**Return value**

Returns a pointer to a null-terminated string containing the hash ID of the source image.

### GetSourceImageTag

Gets the tag of the source image.

```cpp
virtual const CImageTag* GetSourceImageTag() const = 0;
```

**Return value**

Returns a pointer to a CImageTag object representing the tag of the source image.

### GetCount

Gets the number of parsed result items in the parsed result.

```cpp
virtual int GetCount() const = 0;
```

**Return value**

Returns the number of parsed result items in the parsed result.

### GetItem

Gets the parsed result item at the specified index.

```cpp
virtual const CParsedResultItem* GetItem(int index) const = 0;
```

**Parameters**

`[in] index` The zero-based index of the text line result item to retrieve.

**Return value**

Returns a pointer to the `CParsedResultItem` object at the specified index.

### GetErrorCode

Gets the error code of the parsed result, if an error occurred.

```cpp
virtual int GetErrorCode() const = 0;
```

**Return value**

Returns the error code of the parsed result, or 0 if no error occurred.

### GetErrorString

Gets the error message of the parsed result, if an error occurred.

```cpp
virtual const char* GetErrorString() const = 0;
```

**Return value**

Returns a pointer to a null-terminated string containing the error message of the parsed result, or a pointer to an empty string if no error occurred.
