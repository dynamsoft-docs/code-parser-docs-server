---
layout: default-layout
title: ValidationStatus - Dynamsoft Code Parser Java Enumerations
description: The enumeration ValidationStatus of Dynamsoft Code Parser describes the outcome of a validation process on a field.
keywords: Validation status
---

# Enumeration ValidationStatus

`ValidationStatus` describes the outcome of a validation process on a field.

```java
@Retention(RetentionPolicy.CLASS)
public @interface EnumValidationStatus {
    //The field has no validation specified. 
    int VS_NONE = 0;
    //The validation for the field has been succeeded. 
    int VS_SUCCEEDED = 1;
    //The validation for the field has been failed. 
    int VS_FAILED = 2;
}
```
