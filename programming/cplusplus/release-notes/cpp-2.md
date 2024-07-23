---
layout: default-layout
title: Release Notes v2.x - Dynamsoft Code Parser SDK C++ Edition
description: This is the release notes page of Dynamsoft Code Parser SDK C++ Edition v2.x.
keywords: release notes, c++
needGenerateH3Content: false
---

# Release Notes for C++ Edition - 2.x

## 2.4.10 (07/23/2024)

### New

- Added a new function [`AddItem`]({{ site.dcp_cpp_api }}parsed-result.html#additem) to the class [`CParsedResult`]({{ site.dcp_cpp_api }}parsed-result.html).

### Fixed

- Fixed a bug where the South African Driver's License might be parsed incorrectly.

## 2.2.10 (03/01/2024)

### Improved

- Security update for `DynamsoftCodeParser` library and other corresponding libraries.

## 2.2.0 (01/16/2024)

This is a compatibility update that is designed to work with the version 2.2 of `DynamsoftCaptureVision (DCV)` architecture.

### New

- Added the following methods to the `CParsedResult` class:
  - A new constructor
  - `Retain`
  - `Release`

### Breaking Changes

- The destructor functions of the following classes are changed to protected:
  - `CParsedResultItem`
  - `CParsedResult`
- Removed an internal logic that grouping the text line recognition result of the MRZ. The logic is replaced by the text line group definition of the parameter system.
- Change the compiler option of the runtime library of Windows DLLs from MD to MT.

## 2.0.20 (10/26/2023)

This is a compatibility update that is designed to work with the version 2.0.20 of `DynamsoftCaptureVision (DCV)` architecture.

## 2.0.10 (08/08/2023)

### Fixed

* Fixed a bug where the local license is not successfully updated in some cases.
* Fixed crash bugs that happen in rare cases.
* Other small fixes and tweaks.

## 2.0.0 (07/04/2023)

### Highlights

{%- include release-notes/product-highlight-2.0.0.md -%}

