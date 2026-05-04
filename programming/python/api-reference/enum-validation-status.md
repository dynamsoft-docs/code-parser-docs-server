---
layout: default-layout
title: ValidationStatus Enum – Code Parser Python SDK Ref
description: "Explore ValidationStatus values in Dynamsoft Code Parser Python API and learn how they define status, configuration, and processing behavior for modern web."
keywords: Validation status
---

# Enumeration ValidationStatus

`ValidationStatus` describes the outcome of a validation process on a field.

```python
class EnumValidationStatus(IntEnum):
    # The field has no validation specified. 
    VS_NONE
    # The validation for the field has been succeeded. 
    VS_SUCCEEDED
    # The validation for the field has been failed. 
    VS_FAILED
```
