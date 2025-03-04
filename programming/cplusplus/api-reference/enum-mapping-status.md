---
layout: default-layout
title: MappingStatus - Dynamsoft Code Parser Enumerations
description: The enumeration MappingStatus of Dynamsoft Code Parser represents the outcome of a mapping operation on a field.
keywords: Mapping status
---

# Enumeration MappingStatus

`MappingStatus` represents the outcome of a mapping operation on a field.

<div class="sample-code-prefix template2"></div>
   >- C++
   >
>
```cpp
typedef enum MappingStatus
{
   /** The field has no mapping specified. */
   MS_NONE,
   /** Find a mapping for the field value. */
   MS_SUCCEEDED,
   /** Failed to find a mapping for the field value. */
   MS_FAILED
} MappingStatus;
```
