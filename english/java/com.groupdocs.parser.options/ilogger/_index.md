---
title: ILogger
second_title: GroupDocs.Parser for Java API Reference
description: Defines the interface of a logger that is used for logging events and errors during data extraction.
type: docs
weight: 37
url: /java/com.groupdocs.parser.options/ilogger/
---```
public interface ILogger
```

Defines the interface of a logger that is used for logging events and errors during data extraction.

**Learn more:**

 *  [Logging][]


[Logging]: https://docs.groupdocs.com/display/parserjava/Logging
## Methods

| Method | Description |
| --- | --- |
| [error(String message, Exception exception)](#error-java.lang.String-java.lang.Exception-) | Logs an error that occurred during data extraction. |
| [warning(String message)](#warning-java.lang.String-) | Logs a warning that occurred during data extraction. |
| [trace(String message)](#trace-java.lang.String-) | Logs an event occurred during data extraction. |
### error(String message, Exception exception) {#error-java.lang.String-java.lang.Exception-}
```
public abstract void error(String message, Exception exception)
```


Logs an error that occurred during data extraction.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| message | java.lang.String | The error message. |
| exception | java.lang.Exception | The instance of occured exception. |

### warning(String message) {#warning-java.lang.String-}
```
public abstract void warning(String message)
```


Logs a warning that occurred during data extraction.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| message | java.lang.String | The warning message. |

### trace(String message) {#trace-java.lang.String-}
```
public abstract void trace(String message)
```


Logs an event occurred during data extraction.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| message | java.lang.String | The event message. |

