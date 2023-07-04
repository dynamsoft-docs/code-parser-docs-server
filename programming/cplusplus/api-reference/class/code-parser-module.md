---
layout: default-layout
title: CCodeParserModule Class - Dynamsoft Code Parser SDK C++ Edition API Reference
description: This page shows CCodeParserModule Class of Dynamsoft Code Parser SDK C++ Edition.
keywords: CCodeParserModule, api reference, c++
needAutoGenerateSidebar: true
---

# CCodeParserModule Class

  | Method               | Description |
  |----------------------|-------------|
  | [`GetVersion`](#getversion) | Get version information of SDK.|


## GetVersion

Get version information of SDK.

```cpp
static const char* dynamsoft::dcp::CCodeParserModule::GetVersion()
```

**Return Value**

The version information string.

**Code Snippet**

```cpp
const char* versionInfo = dynamsoft::dcp::CCodeParserModule::GetVersion();
```
