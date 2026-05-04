---
layout: default-layout
title: MappingStatus - Dynamsoft Code Parser Python Enumerations
description: "Explore MappingStatus values in Dynamsoft Code Parser Python API and learn how they define status, configuration, and processing behavior for modern web."
keywords: Mapping status
---

# Enumeration MappingStatus

`MappingStatus` represents the outcome of a mapping operation on a field.

```python
class EnumMappingStatus(IntEnum):
    # The field has no mapping specified. 
    MS_NONE
    # Find a mapping for the field value. 
    MS_SUCCEEDED
    # Failed to find a mapping for the field value. 
    MS_FAILED
```
