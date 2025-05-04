---
title: OcrOptions
second_title: GroupDocs.Parser for Java API Reference
description: Provides the options which are used for OCR Connector.
type: docs
weight: 27
url: /java/com.groupdocs.parser.options/ocroptions/
---
**Inheritance:**
java.lang.Object
```
public class OcrOptions
```

Provides the options which are used for OCR Connector.
## Constructors

| Constructor | Description |
| --- | --- |
| [OcrOptions(Rectangle rectangle)](#OcrOptions-com.groupdocs.parser.data.Rectangle-) | Initializes a new instance of the [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with rectangular area. |
| [OcrOptions(OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-) | Initializes a new instance of the [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) object. |
| [OcrOptions(Rectangle rectangle, OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-) | Initializes a new instance of the [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with rectangular area and [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) object. |
| [OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-) | Initializes a new instance of the [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class. |
## Methods

| Method | Description |
| --- | --- |
| [getRectangle()](#getRectangle--) | Gets the rectangular area that constraints the page area which is used for text recognizing. |
| [getHandler()](#getHandler--) | Gets the event handler to catch OCR events. |
| [getUseSpellChecker()](#getUseSpellChecker--) | Gets the value that indicates whether the spell checker is used. |
### OcrOptions(Rectangle rectangle) {#OcrOptions-com.groupdocs.parser.data.Rectangle-}
```
public OcrOptions(Rectangle rectangle)
```


Initializes a new instance of the [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with rectangular area.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | The rectangular area that constraints the page area which is used for text recognizing. |

### OcrOptions(OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(OcrEventHandler handler)
```


Initializes a new instance of the [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | An instance of [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) to catch OCR events. |

### OcrOptions(Rectangle rectangle, OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler)
```


Initializes a new instance of the [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with rectangular area and [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | The rectangular area that constraints the page area which is used for text recognizing. |
| handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | An instance of [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) to catch OCR events. |

### OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)
```


Initializes a new instance of the [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | The rectangular area that constraints the page area which is used for text recognizing. |
| handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | An instance of [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) to catch OCR events. |
| useSpellCheker | boolean | The value that indicates whether the spell checker is used. |

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Gets the rectangular area that constraints the page area which is used for text recognizing.

**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that constraints the page area which is used for text recognizing;  null  if it isn't set.
### getHandler() {#getHandler--}
```
public OcrEventHandler getHandler()
```


Gets the event handler to catch OCR events.

**Returns:**
[OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) - An instance of [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) class which is used to catch OCR events.
### getUseSpellChecker() {#getUseSpellChecker--}
```
public boolean getUseSpellChecker()
```


Gets the value that indicates whether the spell checker is used.

**Returns:**
boolean -  true  if the spell checker is used; otherwise,  false .
