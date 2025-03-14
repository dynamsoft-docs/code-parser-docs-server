---
layout: default-layout
title: CParsedResult Class - Dynamsoft Code Parser SDK C++ Edition API Reference
description: This page shows CParsedResult Class of Dynamsoft Code Parser SDK C++ Edition.
keywords: CParsedResult, api reference, c++
needAutoGenerateSidebar: true
---


# CParsedResult Class

```cpp
class dynamsoft::dcp::CParsedResult : public CCapturedResultBase
```

| Method               | Description |
|----------------------|-------------|
| [`GetItemsCount`](#getitemscount) | Gets the number of parsed result items in the parsed result. |
| [`GetItem`](#getitem) | Gets the parsed result item at the specified index. |
| [`HasItem`](#hasitem) | Check if the item is present in the array. |
| [`RemoveItem`](#removeitem) | Remove a specific item from the array in the parsed results. |
| [`Release`](#release) | Decreases the reference count of the `CParsedResult` object. |
| [`Retain`](#retain) | Increases the reference count of the `CParsedResult` object. |
| [`operator[]`](#operator)           | Gets a pointer to the `CParsedResultItem` object at the specified index.|
| [`AddItem`](#additem) | Adds a specific item to the array in the parsed result. |

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

