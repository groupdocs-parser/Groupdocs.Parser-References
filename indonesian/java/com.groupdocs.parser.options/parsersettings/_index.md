---
title: "ParserSettings"
second_title: "Referensi API GroupDocs.Parser untuk Java"
description: "Menyediakan pengaturan yang digunakan untuk menyesuaikan ekstraksi data."
type: docs
weight: 33
url: /id/java/com.groupdocs.parser.options/parsersettings/
---
**Inheritance:**
java.lang.Object
```
public class ParserSettings
```

Menyediakan pengaturan yang digunakan untuk menyesuaikan ekstraksi data.

**Learn more:**

* [Logging](../https://docs.groupdocs.com/display/parserjava/Logging)

## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
|  | [ParserSettings(ILogger logger)](#ParserSettings-com.groupdocs.parser.options.ILogger-) | Menginisialisasi instance baru dari kelas [ParserSettings](../../com.groupdocs.parser.options/parsersettings) dengan logger. |
|
|  | [ParserSettings(OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-) | Menginisialisasi instance baru dari kelas [ParserSettings](../../com.groupdocs.parser.options/parsersettings) dengan OCR Connector. |
|
|  | [ParserSettings(ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-) | Menginisialisasi instance baru dari kelas [ParserSettings](../../com.groupdocs.parser.options/parsersettings) dengan External Resource Handler. |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-) | Menginisialisasi instance baru dari kelas [ParserSettings](../../com.groupdocs.parser.options/parsersettings) dengan logger dan OCR Connector. |
|
|  | [ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)](#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-) | Menginisialisasi instance baru dari kelas [ParserSettings](../../com.groupdocs.parser.options/parsersettings). |
|
## Metode

| Metode | Deskripsi |
| --- | --- |
|  | [getLogger()](#getLogger--) | Mendapatkan logger yang digunakan untuk mencatat peristiwa dan kesalahan selama ekstraksi data. |
|
|  | [getOcrConnector()](#getOcrConnector--) | Mendapatkan OCR Connector yang digunakan untuk menyediakan fungsi OCR. |
|
|  | [getExternalResourceHandler()](#getExternalResourceHandler--) | Mendapatkan handler untuk sumber daya eksternal. |
|
### ParserSettings(ILogger logger) {#ParserSettings-com.groupdocs.parser.options.ILogger-}
```
public ParserSettings(ILogger logger)
```


Menginisialisasi instance baru dari kelas [ParserSettings](../../com.groupdocs.parser.options/parsersettings) dengan logger.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | Sebuah instance kelas yang mengimplementasikan antarmuka [ILogger](../../com.groupdocs.parser.options/ilogger). |
|

### ParserSettings(OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(OcrConnectorBase ocrConnector)
```


Menginisialisasi instance baru dari kelas [ParserSettings](../../com.groupdocs.parser.options/parsersettings) dengan OCR Connector.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | Sebuah instance kelas yang mewarisi kelas [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) untuk menyediakan fungsi OCR. |
|

### ParserSettings(ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ExternalResourceHandler externalResourceHandler)
```


Menginisialisasi instance baru dari kelas [ParserSettings](../../com.groupdocs.parser.options/parsersettings) dengan External Resource Handler.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | Sebuah instance kelas yang mewarisi kelas [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) untuk menyediakan fungsi OCR. |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)
```


Menginisialisasi instance baru dari kelas [ParserSettings](../../com.groupdocs.parser.options/parsersettings) dengan logger dan OCR Connector.


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | Sebuah instance kelas yang mengimplementasikan antarmuka [ILogger](../../com.groupdocs.parser.options/ilogger). |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | Sebuah instance kelas yang mewarisi kelas [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) untuk menyediakan fungsi OCR. |
|

### ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler) {#ParserSettings-com.groupdocs.parser.options.ILogger-com.groupdocs.parser.options.OcrConnectorBase-com.groupdocs.parser.options.ExternalResourceHandler-}
```
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, ExternalResourceHandler externalResourceHandler)
```


Menginisialisasi instance baru dari kelas [ParserSettings](../../com.groupdocs.parser.options/parsersettings).


**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
|  | logger | [ILogger](../../com.groupdocs.parser.options/ilogger) | Sebuah instance kelas yang mengimplementasikan antarmuka [ILogger](../../com.groupdocs.parser.options/ilogger). |
|
|  | ocrConnector | [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) | Sebuah instance kelas yang mewarisi kelas [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) untuk menyediakan fungsi OCR. |
|
|  | externalResourceHandler | [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) | Sebuah instance kelas yang mewarisi kelas [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) untuk memberikan kontrol atas pemuatan sumber daya eksternal. |
|

### getLogger() {#getLogger--}
```
public ILogger getLogger()
```


Mendapatkan logger yang digunakan untuk mencatat peristiwa dan kesalahan selama ekstraksi data.


**Returns:**
[ILogger](../../com.groupdocs.parser.options/ilogger) - An instance of class that implements [ILogger](../../com.groupdocs.parser.options/ilogger) interface.

### getOcrConnector() {#getOcrConnector--}
```
public OcrConnectorBase getOcrConnector()
```


Mendapatkan OCR Connector yang digunakan untuk menyediakan fungsi OCR.


**Returns:**
[OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) - An instance of class that inherits [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase) class to provide OCR functionality.

### getExternalResourceHandler() {#getExternalResourceHandler--}
```
public ExternalResourceHandler getExternalResourceHandler()
```


Mendapatkan handler untuk sumber daya eksternal.


**Returns:**
[ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) - An instance of class that inherits [ExternalResourceHandler](../../com.groupdocs.parser.options/externalresourcehandler) class to provide the control of external resource loading.

