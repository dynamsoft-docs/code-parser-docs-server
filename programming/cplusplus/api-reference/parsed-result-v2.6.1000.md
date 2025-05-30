---
layout: default-layout
title: CParsedResult Class - Dynamsoft Code Parser SDK C++ Edition API Reference
description: This page shows CParsedResult Class of Dynamsoft Code Parser SDK C++ Edition.
keywords: CParsedResult, api reference, c++
needAutoGenerateSidebar: true
---


# CParsedResult Class

```cpp
class dynamsoft::dcp::CParsedResult
```

| Method               | Description |
|----------------------|-------------|
| [`GetOriginalImageHashId`](#getoriginalimagehashid) | Gets the hash ID of the source image. |
| [`GetOriginalImageTag`](#getoriginalimagetag) | Gets the tag of the source image. |
| [`GetItemsCount`](#getitemscount) | Gets the number of parsed result items in the parsed result. |
| [`GetItem`](#getitem) | Gets the parsed result item at the specified index. |
| [`GetErrorCode`](#geterrorcode) | Gets the error code of the parsed result, if an error occurred. |
| [`GetErrorString`](#geterrorstring) | Gets the error message of the parsed result, if an error occurred. |
| [`HasItem`](#hasitem) | Check if the item is present in the array. |
| [`RemoveItem`](#removeitem) | Remove a specific item from the array in the parsed results. |
| [`Release`](#release) | Decreases the reference count of the `CParsedResult` object. |
| [`Retain`](#retain) | Increases the reference count of the `CParsedResult` object. |
| [`operator[]`](#operator)           | Gets a pointer to the `CParsedResultItem` object at the specified index.|
| [`AddItem`](#additem) | Adds a specific item to the array in the parsed result. |

## GetOriginalImageHashId

Gets the hash ID of the source image.

```cpp
virtual const char* GetOriginalImageHashId() const = 0;
```

**Return value**

Returns a pointer to a null-terminated string containing the hash ID of the source image.

## GetOriginalImageTag

Gets the tag of the source image.

```cpp
virtual const CImageTag* GetOriginalImageTag() const = 0;
```

**Return value**

Returns a pointer to a CImageTag object representing the tag of the source image.

**See Also**

[CImageTag]({{ site.dcvb_cpp_api }}core/basic-structures/image-tag.html)

## GetItemsCount

Gets the number of parsed result items in the parsed result.

```cpp
virtual int GetItemsCount() const = 0;
```

**Return value**

Returns the number of parsed result items in the parsed result.

## GetItem

Gets the parsed result item at the specified index.

```cpp
virtual const CParsedResultItem* GetItem(int index) const = 0;
```

**Parameters**

`[in] index` The zero-based index of the text line result item to retrieve.

**Return value**

Returns a pointer to the `CParsedResultItem` object at the specified index.

**See Also**

[CParsedResultItem]({{ site.dcp_cpp_api }}parsed-result-item.html)

## GetErrorCode

Gets the error code of the parsed result, if an error occurred.

```cpp
virtual int GetErrorCode() const = 0;
```

**Return value**

Returns the error code of the parsed result, or 0 if no error occurred.

## GetErrorString

Gets the error message of the parsed result, if an error occurred.

```cpp
virtual const char* GetErrorString() const = 0;
```

**Return value**

Returns a pointer to a null-terminated string containing the error message of the parsed result, or a pointer to an empty string if no error occurred.

## HasItem

Check if the item is present in the array.

```cpp
virtual bool HasItem(const CParsedResultItem* item) const = 0;
```

**Parameters**

`[in] item` The specific item to be checked.

**Return value**

Returns a bool value indicating whether the item is present in the array or not.

**See Also**

[CParsedResultItem]({{ site.dcp_cpp_api }}parsed-result-item.html)

## RemoveItem

Remove a specific item from the array in the parsed results.

```cpp
virtual int RemoveItem(const CParsedResultItem* item) = 0;
```

**Parameters**

`[in] item` The specific item to be removed.

**Return value**

Returns an error code. Zero indicates success.

**See Also**

[CParsedResultItem]({{ site.dcp_cpp_api }}parsed-result-item.html)


## Release

Decreases the reference count of the `CParsedResult` object.

```cpp
virtual void Release() = 0;
```

## Retain

Increases the reference count of the `CParsedResult` object.

```cpp
virtual CParsedResult* Retain() = 0;
```

**Return value**

Returns an object of `CParsedResult`.

## operator[]

Gets a pointer to the `CParsedResultItem` object at the specified index.

```cpp
virtual const CParsedResultItem* operator[](int index) const = 0;
```

**Parameters**

`[in] index` The index of the parsed result item to retrieve.

**Return value**

Returns a pointer to the `CParsedResultItem` object at the specified index.

**See Also**

[CParsedResultItem]({{ site.dcp_cpp_api }}parsed-result-item.html)

## AddItem

Adds a specific item to the array in the parsed result.

```cpp
virtual int AddItem(const CParsedResultItem* item) = 0;
```

**Parameters**

`[in] item` The specific item to be added.

**Return value**

Returns an error code. Zero indicates success.

**See Also**

[CParsedResultItem]({{ site.dcp_cpp_api }}parsed-result-item.html)

