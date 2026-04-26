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
| [OcrOptions()](#OcrOptions--) | Initializes a new instance of the [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with default values. |
| [OcrOptions(Rectangle rectangle)](#OcrOptions-com.groupdocs.parser.data.Rectangle-) | Initializes a new instance of the [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with rectangular area. |
| [OcrOptions(PagePreviewOptions pagePreviewOptions)](#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-) | Initializes a new instance of the [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with page preview options. |
| [OcrOptions(OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-) | Initializes a new instance of the [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) object. |
| [OcrOptions(Rectangle rectangle, OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-) | Initializes a new instance of the [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with rectangular area and [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) object. |
| [OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-) | Initializes a new instance of the [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class. |
## Methods

| Method | Description |
| --- | --- |
| [getRectangle()](#getRectangle--) | Gets the rectangular area that constraints the page area which is used for text recognizing. |
| [getHandler()](#getHandler--) | Gets the event handler to catch OCR events. |
| [getUseSpellChecker()](#getUseSpellChecker--) | Gets the value that indicates whether the spell checker is used. |
| [getPagePreviewOptions()](#getPagePreviewOptions--) | Gets the page preview options used to render the page that is fed to the OCR engine. |
| [setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)](#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-) | Sets the page preview options used to render the page that is fed to the OCR engine. |
| [getLanguage()](#getLanguage--) | Gets the language used for optical character recognition. |
| [setLanguage(Language language)](#setLanguage-com.groupdocs.parser.options.Language-) | Sets the language used for optical character recognition. |
| [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | Sets the rectangular area that constraints the page area which is used for text recognizing. |
| [setHandler(OcrEventHandler handler)](#setHandler-com.groupdocs.parser.options.OcrEventHandler-) | Sets the event handler to catch OCR events. |
| [setUseSpellChecker(boolean useSpellChecker)](#setUseSpellChecker-boolean-) | Sets the value that indicates whether the spell checker is used. |
### OcrOptions() {#OcrOptions--}
```
public OcrOptions()
```


Initializes a new instance of the [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with default values.

### OcrOptions(Rectangle rectangle) {#OcrOptions-com.groupdocs.parser.data.Rectangle-}
```
public OcrOptions(Rectangle rectangle)
```


Initializes a new instance of the [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with rectangular area.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | The rectangular area that constraints the page area which is used for text recognizing. |

### OcrOptions(PagePreviewOptions pagePreviewOptions) {#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OcrOptions(PagePreviewOptions pagePreviewOptions)
```


Initializes a new instance of the [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with page preview options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | The options used to render the page preview which is fed to the OCR engine. |

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
### getPagePreviewOptions() {#getPagePreviewOptions--}
```
public PagePreviewOptions getPagePreviewOptions()
```


Gets the page preview options used to render the page that is fed to the OCR engine.

**Returns:**
[PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) - The [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions), or  null  if not set.
### setPagePreviewOptions(PagePreviewOptions pagePreviewOptions) {#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public void setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)
```


Sets the page preview options used to render the page that is fed to the OCR engine.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | The page preview options. |

### getLanguage() {#getLanguage--}
```
public Language getLanguage()
```


Gets the language used for optical character recognition.

**Returns:**
[Language](../../com.groupdocs.parser.options/language) - The [Language](../../com.groupdocs.parser.options/language) enum value. Defaults to [Language.Eng](../../com.groupdocs.parser.options/language\#Eng).
### setLanguage(Language language) {#setLanguage-com.groupdocs.parser.options.Language-}
```
public void setLanguage(Language language)
```


Sets the language used for optical character recognition.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| language | [Language](../../com.groupdocs.parser.options/language) | The [Language](../../com.groupdocs.parser.options/language) enum value. |

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


Sets the rectangular area that constraints the page area which is used for text recognizing.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | The rectangle, or  null  to scan the whole page. |

### setHandler(OcrEventHandler handler) {#setHandler-com.groupdocs.parser.options.OcrEventHandler-}
```
public void setHandler(OcrEventHandler handler)
```


Sets the event handler to catch OCR events.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | The event handler. |

### setUseSpellChecker(boolean useSpellChecker) {#setUseSpellChecker-boolean-}
```
public void setUseSpellChecker(boolean useSpellChecker)
```


Sets the value that indicates whether the spell checker is used.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| useSpellChecker | boolean |  true  to enable spell checking. |

