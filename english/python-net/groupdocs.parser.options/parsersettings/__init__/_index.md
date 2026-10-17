---
title: __init__ constructor
second_title: GroupDocs.Parser for Python via .NET API References
description: "Initializes a new instance of the ParserSettings class with the logger."
type: docs
url: /python-net/groupdocs.parser.options/parsersettings/__init__/
is_root: false
weight: 10
---


## __init__ {#logger}

Initializes a new instance of the [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings/) class with the logger.

```python
def __init__(self, logger):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| logger | `ILogger` | An instance of a class that implements the `ILogger` interface. |

## __init__ {#ocr_connector}

Initializes a new instance of the [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings/) class with the OCR connector.

```python
def __init__(self, ocr_connector):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| ocr_connector | `OcrConnectorBase` | An instance of a class that inherits `OcrConnectorBase` to provide OCR functionality. |

## __init__ {#external_resource_handler}

Initializes a new instance of the [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings/) class with the external resource handler.

```python
def __init__(self, external_resource_handler):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| external_resource_handler | `ExternalResourceHandler` | An instance of a class that inherits `ExternalResourceHandler` to provide control of external resources loading. |

## __init__ {#logger-ocr_connector}

Initializes a new ParserSettings instance with a logger and an OCR connector.

```python
def __init__(self, logger, ocr_connector):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| logger | `ILogger` | An instance of a class that implements `ILogger`. |
| ocr_connector | `OcrConnectorBase` | An instance of a class that inherits `OcrConnectorBase` to provide OCR functionality. |

## __init__ {#logger-ocr_connector-external_resource_handler}

Initializes a new instance of the ParserSettings class with logger, OCR Connector and External Resource Handler.

```python
def __init__(self, logger, ocr_connector, external_resource_handler):
    ...
```

| Parameter | Type | Description |
| :- | :- | :- |
| logger | `ILogger` | An instance of class that implements `ILogger` interface. |
| ocr_connector | `OcrConnectorBase` | An instance of class that inherits `OcrConnectorBase` class to provide OCR functionality. |
| external_resource_handler | `ExternalResourceHandler` | An instance of class that inherits `ExternalResourceHandler` class to provide the control of external resource loading. |

### See Also
* class [`ParserSettings`](/parser/python-net/groupdocs.parser.options/parsersettings/)
