---
layout: default-layout
title: CodeParser Class - Dynamsoft Code Parser Module Java Edition API Reference
description: Definition of the CodeParser class in Dynamsoft Code Parser Module Java Edition.
keywords: CodeParser, api reference, java
needAutoGenerateSidebar: true
---

# CodeParser Class

The `CodeParser` class provides functionality for parsing codes from byte data.

## Definition

*Package:* com.dynamsoft.dcp

```java
public class CodeParser
```

## Constructors

| Constructor               | Description |
|---------------------------|-------------|
| [`CodeParser`](#codeparser) | Constructor to create a new CodeParser instance.|

## Methods

| Method               | Description |
|----------------------|-------------|
| [`Parse`](#parse) | Parses code from byte data. |
| [`InitSettings`](#initsettings) | Initializes the code parser with JSON settings. |
| [`InitSettingsFromFile`](#initsettingsfromfile) | Initializes the code parser with settings from a file. |
| [`ResetSettings`](#resetsettings) | Resets the code parser settings to default. |

### CodeParser

Constructor to create a new CodeParser instance.

```java
public CodeParser()
```

### Parse

Parses code from byte data.

```java
public ParsedResultItem Parse(byte[] data) throws CodeParserException
```

**Parameters**

`data` The byte array containing the data to parse.

**Return Value**

Returns a `ParsedResultItem` object containing the parsed result.

**Exceptions**

`CodeParserException` Thrown when an error occurs during parsing.

**See Also**

[ParsedResultItem]({{ site.dcp_java_api }}parsed-result-item.html)
[CodeParserException]({{ site.dcp_java_api }}code-parser-exception.html)

---

```java
public ParsedResultItem Parse(byte[] data, String taskSettingName) throws CodeParserException
```

**Parameters**

`data` The byte array containing the data to parse.
`taskSettingName` The name of the task setting to use for parsing.

**Return Value**

Returns a `ParsedResultItem` object containing the parsed result.

**Exceptions**

`CodeParserException` Thrown when an error occurs during parsing.

**See Also**

[ParsedResultItem]({{ site.dcp_java_api }}parsed-result-item.html)
[CodeParserException]({{ site.dcp_java_api }}code-parser-exception.html)

### InitSettings

Initializes the code parser with JSON settings.

```java
public void InitSettings(String content) throws CodeParserException
```

**Parameters**

`content` A JSON string containing the settings.

**Exceptions**

`CodeParserException` Thrown when an error occurs during initialization.

**See Also**

[CodeParserException]({{ site.dcp_java_api }}code-parser-exception.html)

### InitSettingsFromFile

Initializes the code parser with settings from a file.

```java
public void InitSettingsFromFile(String filePath) throws CodeParserException
```

**Parameters**

`filePath` The path to the file containing the settings.

**Exceptions**

`CodeParserException` Thrown when an error occurs during initialization.

**See Also**

[CodeParserException]({{ site.dcp_java_api }}code-parser-exception.html)

### ResetSettings

Resets the code parser settings to default.

```java
public void ResetSettings() throws CodeParserException
```

**Exceptions**

`CodeParserException` Thrown when an error occurs during reset.

**See Also**

[CodeParserException]({{ site.dcp_java_api }}code-parser-exception.html)
