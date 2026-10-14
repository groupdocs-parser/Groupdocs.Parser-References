---
title: "ILogger"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "데이터 추출 중 이벤트와 오류를 기록하는 데 사용되는 로거의 인터페이스를 정의합니다."
type: docs
weight: 40
url: /ko/java/com.groupdocs.parser.options/ilogger/
---```
public interface ILogger
```

Defines the interface of a logger that is used for logging events and errors during data extraction.

**Learn more:**

* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

## Methods

| Method | Description |
| --- | --- |
| [error(String message, Exception exception)](#error-java.lang.String-java.lang.Exception-) | Logs an error that occurred during data extraction.
 |
| [warning(String message)](#warning-java.lang.String-) | Logs a warning that occurred during data extraction.
 |
| [trace(String message)](#trace-java.lang.String-) | Logs an event occurred during data extraction.
 |
### error(String message, Exception exception) {#error-java.lang.String-java.lang.Exception-}
```
public abstract void error(String message, Exception exception)
```


Logs an error that occurred during data extraction.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| message | java.lang.String | The error message.
 |
| exception | java.lang.Exception | The instance of occured exception.
 |

### warning(String message) {#warning-java.lang.String-}
```
public abstract void warning(String message)
```


Logs a warning that occurred during data extraction.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| message | java.lang.String | The warning message.
 |

### trace(String message) {#trace-java.lang.String-}
```
public abstract void trace(String message)
```


Logs an event occurred during data extraction.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| message | java.lang.String | The event message.
 |

