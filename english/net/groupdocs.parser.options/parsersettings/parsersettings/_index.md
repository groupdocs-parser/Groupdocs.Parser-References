---
title: ParserSettings
second_title: GroupDocs.Parser for .NET API Reference
description: Initializes a new instance of the ParserSettingsgroupdocs.parser.options/parsersettings class with the page preview options.
type: docs
weight: 10
url: /net/groupdocs.parser.options/parsersettings/parsersettings/
---
## ParserSettings(PagePreviewOptions) {#constructor_9}

Initializes a new instance of the [`ParserSettings`](../../parsersettings) class with the page preview options.

```csharp
public ParserSettings(PagePreviewOptions pagePreviewOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| pagePreviewOptions | PagePreviewOptions | An instance of [`PagePreviewOptions`](../pagepreviewoptions) class that sets properties for the document page preview generation. It's used in the barcode extraction and OCR. |

### See Also

* class [PagePreviewOptions](../../pagepreviewoptions)
* class [ParserSettings](../../parsersettings)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## ParserSettings(ILogger) {#constructor_1}

Initializes a new instance of the [`ParserSettings`](../../parsersettings) class with the logger.

```csharp
public ParserSettings(ILogger logger)
```

| Parameter | Type | Description |
| --- | --- | --- |
| logger | ILogger | An instance of class that implements [`ILogger`](../../ilogger) interface. |

### See Also

* interface [ILogger](../../ilogger)
* class [ParserSettings](../../parsersettings)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## ParserSettings(ILogger, PagePreviewOptions) {#constructor_6}

Initializes a new instance of the [`ParserSettings`](../../parsersettings) class with the logger and page preview options.

```csharp
public ParserSettings(ILogger logger, PagePreviewOptions pagePreviewOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| logger | ILogger | An instance of class that implements [`ILogger`](../../ilogger) interface. |
| pagePreviewOptions | PagePreviewOptions | An instance of [`PagePreviewOptions`](../pagepreviewoptions) class that sets properties for the document page preview generation. It's used in the barcode extraction and OCR. |

### See Also

* interface [ILogger](../../ilogger)
* class [PagePreviewOptions](../../pagepreviewoptions)
* class [ParserSettings](../../parsersettings)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## ParserSettings(OcrConnectorBase) {#constructor_7}

Initializes a new instance of the [`ParserSettings`](../../parsersettings) class with the OCR Connector.

```csharp
public ParserSettings(OcrConnectorBase ocrConnector)
```

| Parameter | Type | Description |
| --- | --- | --- |
| ocrConnector | OcrConnectorBase | An instance of class that inherits [`OcrConnectorBase`](../../ocrconnectorbase) class to provide OCR functionality. |

### See Also

* class [OcrConnectorBase](../../ocrconnectorbase)
* class [ParserSettings](../../parsersettings)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## ParserSettings(OcrConnectorBase, PagePreviewOptions) {#constructor_8}

Initializes a new instance of the [`ParserSettings`](../../parsersettings) class with the OCR Connector and page preview options.

```csharp
public ParserSettings(OcrConnectorBase ocrConnector, PagePreviewOptions pagePreviewOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| ocrConnector | OcrConnectorBase | An instance of class that inherits [`OcrConnectorBase`](../../ocrconnectorbase) class to provide OCR functionality. |
| pagePreviewOptions | PagePreviewOptions | An instance of [`PagePreviewOptions`](../pagepreviewoptions) class that sets properties for the document page preview generation. It's used in the barcode extraction and OCR. |

### See Also

* class [OcrConnectorBase](../../ocrconnectorbase)
* class [PagePreviewOptions](../../pagepreviewoptions)
* class [ParserSettings](../../parsersettings)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## ParserSettings(ExternalResourceHandler) {#constructor}

Initializes a new instance of the [`ParserSettings`](../../parsersettings) class with the External Resource Handler.

```csharp
public ParserSettings(ExternalResourceHandler externalResourceHandler)
```

| Parameter | Type | Description |
| --- | --- | --- |
| externalResourceHandler | ExternalResourceHandler | An instance of class that inherits [`ExternalResourceHandler`](../../externalresourcehandler) class to provide the control of external resources loading. |

### See Also

* class [ExternalResourceHandler](../../externalresourcehandler)
* class [ParserSettings](../../parsersettings)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## ParserSettings(ILogger, OcrConnectorBase) {#constructor_2}

Initializes a new instance of the [`ParserSettings`](../../parsersettings) class with logger and OCR Connector.

```csharp
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector)
```

| Parameter | Type | Description |
| --- | --- | --- |
| logger | ILogger | An instance of class that implements [`ILogger`](../../ilogger) interface. |
| ocrConnector | OcrConnectorBase | An instance of class that inherits [`OcrConnectorBase`](../../ocrconnectorbase) class to provide OCR functionality. |

### See Also

* interface [ILogger](../../ilogger)
* class [OcrConnectorBase](../../ocrconnectorbase)
* class [ParserSettings](../../parsersettings)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## ParserSettings(ILogger, OcrConnectorBase, PagePreviewOptions) {#constructor_5}

Initializes a new instance of the [`ParserSettings`](../../parsersettings) class with logger, OCR Connector and page preview options.

```csharp
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, 
    PagePreviewOptions pagePreviewOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| logger | ILogger | An instance of class that implements [`ILogger`](../../ilogger) interface. |
| ocrConnector | OcrConnectorBase | An instance of class that inherits [`OcrConnectorBase`](../../ocrconnectorbase) class to provide OCR functionality. |
| pagePreviewOptions | PagePreviewOptions | An instance of [`PagePreviewOptions`](../pagepreviewoptions) class that sets properties for the document page preview generation. It's used in the barcode extraction and OCR. |

### See Also

* interface [ILogger](../../ilogger)
* class [OcrConnectorBase](../../ocrconnectorbase)
* class [PagePreviewOptions](../../pagepreviewoptions)
* class [ParserSettings](../../parsersettings)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## ParserSettings(ILogger, OcrConnectorBase, ExternalResourceHandler) {#constructor_3}

Initializes a new instance of the [`ParserSettings`](../../parsersettings) class with logger, OCR Connector and External Resource Handler.

```csharp
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, 
    ExternalResourceHandler externalResourceHandler)
```

| Parameter | Type | Description |
| --- | --- | --- |
| logger | ILogger | An instance of class that implements [`ILogger`](../../ilogger) interface. |
| ocrConnector | OcrConnectorBase | An instance of class that inherits [`OcrConnectorBase`](../../ocrconnectorbase) class to provide OCR functionality. |
| externalResourceHandler | ExternalResourceHandler | An instance of class that inherits [`ExternalResourceHandler`](../../externalresourcehandler) class to provide the control of external resource loading. |

### See Also

* interface [ILogger](../../ilogger)
* class [OcrConnectorBase](../../ocrconnectorbase)
* class [ExternalResourceHandler](../../externalresourcehandler)
* class [ParserSettings](../../parsersettings)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## ParserSettings(ILogger, OcrConnectorBase, ExternalResourceHandler, PagePreviewOptions) {#constructor_4}

Initializes a new instance of the [`ParserSettings`](../../parsersettings) class.

```csharp
public ParserSettings(ILogger logger, OcrConnectorBase ocrConnector, 
    ExternalResourceHandler externalResourceHandler, PagePreviewOptions pagePreviewOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| logger | ILogger | An instance of class that implements [`ILogger`](../../ilogger) interface. |
| ocrConnector | OcrConnectorBase | An instance of class that inherits [`OcrConnectorBase`](../../ocrconnectorbase) class to provide OCR functionality. |
| externalResourceHandler | ExternalResourceHandler | An instance of class that inherits [`ExternalResourceHandler`](../../externalresourcehandler) class to provide the control of external resource loading. |
| pagePreviewOptions | PagePreviewOptions | An instance of [`PagePreviewOptions`](../pagepreviewoptions) class that sets properties for the document page preview generation. It's used in the barcode extraction and OCR. |

### See Also

* interface [ILogger](../../ilogger)
* class [OcrConnectorBase](../../ocrconnectorbase)
* class [ExternalResourceHandler](../../externalresourcehandler)
* class [PagePreviewOptions](../../pagepreviewoptions)
* class [ParserSettings](../../parsersettings)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.parser.dll -->
