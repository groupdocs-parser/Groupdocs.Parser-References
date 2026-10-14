---
title: "ParserSettings"
second_title: "مرجع API لـ GroupDocs.Parser للغة Java"
description: "يوفر الإعدادات المستخدمة لتخصيص استخراج البيانات."
type: docs
weight: 33
url: /ar/java/com.groupdocs.parser.options/parsersettings/
---
**Inheritance:**
java.lang.Object
```
public class ParserSettings
```

يوفر الإعدادات المستخدمة لتخصيص استخراج البيانات.

**Learn more:**

* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

## البناؤات

| البناء | الوصف |
| --- | --- |
|  | [ParserSettings(ILogger logger)](#ParserSettings-com.groupdocs.parser.options.ILogger-) | يقوم بإنشاء نسخة جديدة من الفئة [ParserSettings](../../com.groupdocs.parser.options/parsersettings) مع المُسجل. |
|
|  | [ParserSettings(OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-) | يقوم بإنشاء نسخة جديدة من الفئة [ParserSettings](../../com.groupdocs.parser.options/parsersettings) مع موصل OCR. |
|
|  | [ParserSettings(ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-) | يقوم بإنشاء نسخة جديدة من الفئة [ParserSettings](../../com.groupdocs.parser.options/parsersettings) مع معالج الموارد الخارجية. |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-) | يقوم بإنشاء نسخة جديدة من الفئة [ParserSettings](../../com.groupdocs.parser.options/parsersettings) مع المُسجل وموصل OCR. |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-) | يقوم بإنشاء نسخة جديدة من الفئة [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
## الطرق

| الطريقة | الوصف |
| --- | --- |
|  | [getLogger()](#getLogger--) | يحصل على المُسجل الذي يُستخدم لتسجيل الأحداث والأخطاء أثناء استخراج البيانات. |
|
|  | [getOcrConnector()](#getOcrConnector--) | يحصل على موصل OCR الذي يُستخدم لتوفير وظيفة OCR. |
|
|  | [getExternalResourceHandler()](#getExternalResourceHandler--) | يحصل على المعالج للموارد الخارجية. |
|
### ParserSettings(ILogger logger) {#ParserSettings-com.groupdocs.parser.options.ILogger-}
```
public ParserSettings(ILogger logger)
```


يقوم بإنشاء نسخة جديدة من الفئة [ParserSettings](../../com.groupdocs.parser.options/parsersettings) مع المُسجل.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | مثيل من الفئة التي تنفّذ واجهة [ILogger](../../com.groupdocs.parser.options/ilogger). |
|

### ParserSettings(OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(OcrConnectorBase ocrConnector)
```


يقوم بإنشاء نسخة جديدة من الفئة [ParserSettings](../../com.groupdocs.parser.options/parsersettings) مع موصل OCR.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | مثيل من الفئة التي ترث الفئة [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) لتوفير وظيفة OCR. |
|

### ParserSettings(ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ExternalResourceHandler externalResourceHandler)
```


يقوم بإنشاء نسخة جديدة من الفئة [ParserSettings](../../com.groupdocs.parser.options/parsersettings) مع معالج الموارد الخارجية.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | مثيل من الفئة التي ترث الفئة [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) لتوفير وظيفة OCR. |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)
```


يقوم بإنشاء نسخة جديدة من الفئة [ParserSettings](../../com.groupdocs.parser.options/parsersettings) مع المُسجل وموصل OCR.


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | مثيل من الفئة التي تنفّذ واجهة [ILogger](../../com.groupdocs.parser.options/ilogger). |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | مثيل من الفئة التي ترث الفئة [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) لتوفير وظيفة OCR. |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)
```


يقوم بإنشاء نسخة جديدة من الفئة [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| المعامل | النوع | الوصف |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | مثيل من الفئة التي تنفّذ واجهة [ILogger](../../com.groupdocs.parser.options/ilogger). |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | مثيل من الفئة التي ترث الفئة [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) لتوفير وظيفة OCR. |
|
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | مثيل من الفئة التي ترث الفئة [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) لتوفير التحكم في تحميل الموارد الخارجية. |
|

### getLogger() {#getLogger--}
```
public ILogger getLogger()
```


يحصل على المُسجل الذي يُستخدم لتسجيل الأحداث والأخطاء أثناء استخراج البيانات.


**Returns:**
[ILogger](../../com.groupdocs.parser.options/ilogger) - An instance of class that implements [ILogger](../../com.groupdocs.parser.options/ilogger) interface.

### getOcrConnector() {#getOcrConnector--}
```
public OcrConnectorBase getOcrConnector()
```


يحصل على موصل OCR الذي يُستخدم لتوفير وظيفة OCR.


**Returns:**
[OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) - An instance of class that inherits [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) class to provide OCR functionality.

### getExternalResourceHandler() {#getExternalResourceHandler--}
```
public ExternalResourceHandler getExternalResourceHandler()
```


يحصل على المعالج للموارد الخارجية.


**Returns:**
[ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) - An instance of class that inherits [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) class to provide the control of external resource loading.

