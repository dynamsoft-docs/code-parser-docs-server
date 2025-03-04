---
layout: default-layout
title: ValidationStatus - Dynamsoft Code Parser Enumerations
description: The enumeration ValidationStatus of Dynamsoft Code Parser describes the outcome of a validation process on a field.
keywords: Validation status
---

# Enumeration ValidationStatus

`ValidationStatus` describes the outcome of a validation process on a field.

<div class="sample-code-prefix template2"></div>
   >- C++
   >
>
```cpp
typedef enum ValidationStatus
{
   /** The field has no validation specified. */
   VS_NONE,
   /** The validation for the field has been succeeded. */
   VS_SUCCEEDED,
   /** The validation for the field has been failed. */
   VS_FAILED
} ValidationStatus;
```
