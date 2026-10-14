---
title: "ParserSettings"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "데이터 추출을 사용자 정의하는 데 사용되는 설정을 제공합니다."
type: docs
weight: 33
url: /ko/java/com.groupdocs.parser.options/parsersettings/
---
**Inheritance:**
java.lang.Object
```
public class ParserSettings
```

데이터 추출을 사용자 정의하는 데 사용되는 설정을 제공합니다.

**Learn more:**

* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

## 생성자

| 생성자 | 설명 |
| --- | --- |
|  | [ParserSettings(ILogger logger)](#ParserSettings-com.groupdocs.parser.options.ILogger-) | 로거와 함께 새로운 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 클래스 인스턴스를 초기화합니다. |
|
|  | [ParserSettings(OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-) | OCR 커넥터와 함께 새로운 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 클래스 인스턴스를 초기화합니다. |
|
|  | [ParserSettings(ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-) | 외부 리소스 핸들러와 함께 새로운 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 클래스 인스턴스를 초기화합니다. |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-) | 로거와 OCR 커넥터와 함께 새로운 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 클래스 인스턴스를 초기화합니다. |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-) | 새로운 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 클래스 인스턴스를 초기화합니다. |
|
## 메서드

| 메서드 | 설명 |
| --- | --- |
|  | [getLogger()](#getLogger--) | 데이터 추출 중 이벤트와 오류를 기록하는 데 사용되는 로거를 가져옵니다. |
|
|  | [getOcrConnector()](#getOcrConnector--) | OCR 기능을 제공하는 OCR 커넥터를 가져옵니다. |
|
|  | [getExternalResourceHandler()](#getExternalResourceHandler--) | 외부 리소스용 핸들러를 가져옵니다. |
|
### ParserSettings(ILogger logger) {#ParserSettings-com.groupdocs.parser.options.ILogger-}
```
public ParserSettings(ILogger logger)
```


로거와 함께 새로운 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | [ILogger](../../com.groupdocs.parser.options/ilogger) 인터페이스를 구현하는 클래스의 인스턴스입니다. |
|

### ParserSettings(OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(OcrConnectorBase ocrConnector)
```


OCR 커넥터와 함께 새로운 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | OCR 기능을 제공하기 위해 [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) 클래스를 상속하는 클래스의 인스턴스입니다. |
|

### ParserSettings(ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ExternalResourceHandler externalResourceHandler)
```


외부 리소스 핸들러와 함께 새로운 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | OCR 기능을 제공하기 위해 [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) 클래스를 상속하는 클래스의 인스턴스입니다. |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)
```


로거와 OCR 커넥터와 함께 새로운 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | [ILogger](../../com.groupdocs.parser.options/ilogger) 인터페이스를 구현하는 클래스의 인스턴스입니다. |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | OCR 기능을 제공하기 위해 [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) 클래스를 상속하는 클래스의 인스턴스입니다. |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)
```


새로운 [ParserSettings](../../com.groupdocs.parser.options/parsersettings) 클래스 인스턴스를 초기화합니다.


**Parameters:**
| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | [ILogger](../../com.groupdocs.parser.options/ilogger) 인터페이스를 구현하는 클래스의 인스턴스입니다. |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | OCR 기능을 제공하기 위해 [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) 클래스를 상속하는 클래스의 인스턴스입니다. |
|
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | 외부 리소스 로딩 제어를 제공하기 위해 [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) 클래스를 상속하는 클래스의 인스턴스입니다. |
|

### getLogger() {#getLogger--}
```
public ILogger getLogger()
```


데이터 추출 중 이벤트와 오류를 기록하는 데 사용되는 로거를 가져옵니다.


**Returns:**
[ILogger](../../com.groupdocs.parser.options/ilogger) - An instance of class that implements [ILogger](../../com.groupdocs.parser.options/ilogger) interface.

### getOcrConnector() {#getOcrConnector--}
```
public OcrConnectorBase getOcrConnector()
```


OCR 기능을 제공하는 OCR 커넥터를 가져옵니다.


**Returns:**
[OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) - An instance of class that inherits [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) class to provide OCR functionality.

### getExternalResourceHandler() {#getExternalResourceHandler--}
```
public ExternalResourceHandler getExternalResourceHandler()
```


외부 리소스용 핸들러를 가져옵니다.


**Returns:**
[ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) - An instance of class that inherits [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) class to provide the control of external resource loading.

