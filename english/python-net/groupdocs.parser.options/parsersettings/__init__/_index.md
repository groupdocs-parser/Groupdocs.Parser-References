---
title: ParserSettings constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: 
type: docs
url: /python-net/groupdocs.parser.options/parsersettings/__init__/
is_root: false
weight: 10
---

## __init__ {#groupdocs.parser.options.ILogger}

Initializes a new instance of the [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings) class with the logger.



```python
def __init__(self, logger):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| logger | groupdocs.parser.options.ILogger | An instance of class that implements [`ILogger`](/parser/python-net/groupdocs.parser.options/ilogger) interface. |


## __init__ {#groupdocs.parser.options.OcrConnectorBase}

Initializes a new instance of the [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings) class with the OCR Connector.



```python
def __init__(self, ocr_connector):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| ocr_connector | groupdocs.parser.options.OcrConnectorBase | An instance of class that inherits [`OcrConnectorBase`](/parser/python-net/groupdocs.parser.options/ocrconnectorbase) class to provide OCR functionality. |


## __init__ {#groupdocs.parser.options.ExternalResourceHandler}

Initializes a new instance of the [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings) class with the External Resource Handler.



```python
def __init__(self, external_resource_handler):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| external_resource_handler | groupdocs.parser.options.ExternalResourceHandler | An instance of class that inherits [`ExternalResourceHandler`](/parser/python-net/groupdocs.parser.options/externalresourcehandler) class to provide the control of external resources loading. |


## __init__ {#groupdocs.parser.options.ILogger-groupdocs.parser.options.OcrConnectorBase}

Initializes a new instance of the [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings) class with logger and OCR Connector.



```python
def __init__(self, logger, ocr_connector):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| logger | groupdocs.parser.options.ILogger | An instance of class that implements [`ILogger`](/parser/python-net/groupdocs.parser.options/ilogger) interface. |
| ocr_connector | groupdocs.parser.options.OcrConnectorBase | An instance of class that inherits [`OcrConnectorBase`](/parser/python-net/groupdocs.parser.options/ocrconnectorbase) class to provide OCR functionality. |


## __init__ {#groupdocs.parser.options.ILogger-groupdocs.parser.options.OcrConnectorBase-groupdocs.parser.options.ExternalResourceHandler}

Initializes a new instance of the [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings) class with logger, OCR Connector and External Resource Handler.



```python
def __init__(self, logger, ocr_connector, external_resource_handler):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| logger | groupdocs.parser.options.ILogger | An instance of class that implements [`ILogger`](/parser/python-net/groupdocs.parser.options/ilogger) interface. |
| ocr_connector | groupdocs.parser.options.OcrConnectorBase | An instance of class that inherits [`OcrConnectorBase`](/parser/python-net/groupdocs.parser.options/ocrconnectorbase) class to provide OCR functionality. |
| external_resource_handler | groupdocs.parser.options.ExternalResourceHandler | An instance of class that inherits [`ExternalResourceHandler`](/parser/python-net/groupdocs.parser.options/externalresourcehandler) class to provide the control of external resource loading. |



### See Also
* module [`groupdocs.parser.options`](../../)
* class [`ExternalResourceHandler`](/parser/python-net/groupdocs.parser.options/externalresourcehandler)
* class [`ILogger`](/parser/python-net/groupdocs.parser.options/ilogger)
* class [`OcrConnectorBase`](/parser/python-net/groupdocs.parser.options/ocrconnectorbase)
* class [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings)
