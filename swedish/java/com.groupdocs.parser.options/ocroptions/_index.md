---
title: "OcrOptions"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller de alternativ som används för OCR-Connector."
type: docs
weight: 27
url: /sv/java/com.groupdocs.parser.options/ocroptions/
---
**Inheritance:**
java.lang.Object
```
public class OcrOptions
```

Tillhandahåller de alternativ som används för OCR-Connector.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [OcrOptions()](#OcrOptions--) | Initierar en ny instans av klassen [OcrOptions](../../com.groupdocs.parser.options/ocroptions) med standardvärden. |
|
|  | [OcrOptions(Rectangle rectangle)](#OcrOptions-com.groupdocs.parser.data.Rectangle-) | Initierar en ny instans av klassen [OcrOptions](../../com.groupdocs.parser.options/ocroptions) med rektangulärt område. |
|
|  | [OcrOptions(PagePreviewOptions pagePreviewOptions)](#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-) | Initierar en ny instans av klassen [OcrOptions](../../com.groupdocs.parser.options/ocroptions) med alternativ för sidförhandsgranskning. |
|
|  | [OcrOptions(OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-) | Initierar en ny instans av klassen [OcrOptions](../../com.groupdocs.parser.options/ocroptions) med objektet [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler). |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-) | Initierar en ny instans av klassen [OcrOptions](../../com.groupdocs.parser.options/ocroptions) med rektangulärt område och objektet [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler). |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-) | Initierar en ny instans av klassen [OcrOptions](../../com.groupdocs.parser.options/ocroptions). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Hämtar det rektangulära området som begränsar sidområdet som används för textigenkänning. |
|
|  | [getHandler()](#getHandler--) | Hämtar händelsehanteraren för att fånga OCR‑händelser. |
|
|  | [getUseSpellChecker()](#getUseSpellChecker--) | Hämtar värdet som indikerar om stavningskontrollen används. |
|
|  | [getPagePreviewOptions()](#getPagePreviewOptions--) | Hämtar förhandsgranskningsalternativen för sidan som används för att rendera sidan som matas till OCR-motorn. |
|
|  | [setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)](#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-) | Ställer in förhandsgranskningsalternativen för sidan som används för att rendera sidan som matas till OCR-motorn. |
|
|  | [getLanguage()](#getLanguage--) | Hämtar språket som används för optisk teckenigenkänning. |
|
|  | [setLanguage(Language language)](#setLanguage-com.groupdocs.parser.options.Language-) | Ställer in språket som används för optisk teckenigenkänning. |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | Ställer in det rektangulära området som begränsar sidområdet som används för textigenkänning. |
|
|  | [setHandler(OcrEventHandler handler)](#setHandler-com.groupdocs.parser.options.OcrEventHandler-) | Ställer in händelsehanteraren för att fånga OCR‑händelser. |
|
|  | [setUseSpellChecker(boolean useSpellChecker)](#setUseSpellChecker-boolean-) | Ställer in värdet som indikerar om stavningskontrollen används. |
|
### OcrOptions() {#OcrOptions--}
```
public OcrOptions()
```


Initierar en ny instans av klassen [OcrOptions](../../com.groupdocs.parser.options/ocroptions) med standardvärden.


### OcrOptions(Rectangle rectangle) {#OcrOptions-com.groupdocs.parser.data.Rectangle-}
```
public OcrOptions(Rectangle rectangle)
```


Initierar en ny instans av klassen [OcrOptions](../../com.groupdocs.parser.options/ocroptions) med rektangulärt område.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området som begränsar sidområdet som används för textigenkänning. |
|

### OcrOptions(PagePreviewOptions pagePreviewOptions) {#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OcrOptions(PagePreviewOptions pagePreviewOptions)
```


Initierar en ny instans av klassen [OcrOptions](../../com.groupdocs.parser.options/ocroptions) med alternativ för sidförhandsgranskning.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | Alternativen som används för att rendera förhandsgranskningen av sidan som matas till OCR-motorn. |
|

### OcrOptions(OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(OcrEventHandler handler)
```


Initierar en ny instans av klassen [OcrOptions](../../com.groupdocs.parser.options/ocroptions) med objektet [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | En instans av [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) för att fånga OCR‑händelser. |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler)
```


Initierar en ny instans av klassen [OcrOptions](../../com.groupdocs.parser.options/ocroptions) med rektangulärt område och objektet [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området som begränsar sidområdet som används för textigenkänning. |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | En instans av [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) för att fånga OCR‑händelser. |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)
```


Initierar en ny instans av klassen [OcrOptions](../../com.groupdocs.parser.options/ocroptions).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området som begränsar sidområdet som används för textigenkänning. |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | En instans av [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) för att fånga OCR‑händelser. |
|
|  | useSpellCheker | boolean | Värdet som indikerar om stavningskontrollen används. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Hämtar det rektangulära området som begränsar sidområdet som används för textigenkänning.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that constraints the page area which is used for text recognizing;  null  if it isn't set.

### getHandler() {#getHandler--}
```
public OcrEventHandler getHandler()
```


Hämtar händelsehanteraren för att fånga OCR‑händelser.


**Returns:**
[OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) - An instance of [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) class which is used to catch OCR events.

### getUseSpellChecker() {#getUseSpellChecker--}
```
public boolean getUseSpellChecker()
```


Hämtar värdet som indikerar om stavningskontrollen används.


**Returns:**
boolean -  true  om stavningskontrollen används; annars,  false .

### getPagePreviewOptions() {#getPagePreviewOptions--}
```
public PagePreviewOptions getPagePreviewOptions()
```


Hämtar förhandsgranskningsalternativen för sidan som används för att rendera sidan som matas till OCR-motorn.


**Returns:**
[PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) - The [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions), or  null  if not set.

### setPagePreviewOptions(PagePreviewOptions pagePreviewOptions) {#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public void setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)
```


Ställer in förhandsgranskningsalternativen för sidan som används för att rendera sidan som matas till OCR-motorn.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | Förhandsgranskningsalternativen för sidan. |
|

### getLanguage() {#getLanguage--}
```
public Language getLanguage()
```


Hämtar språket som används för optisk teckenigenkänning.


**Returns:**
[Language](../../com.groupdocs.parser.options/language) - The [Language](../../com.groupdocs.parser.options/language) enum value. Defaults to [Language.Eng](../../com.groupdocs.parser.options/language#Eng).

### setLanguage(Language language) {#setLanguage-com.groupdocs.parser.options.Language-}
```
public void setLanguage(Language language)
```


Ställer in språket som används för optisk teckenigenkänning.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | language | [Language](../../com.groupdocs.parser.options/language) | Enum‑värdet [Language](../../com.groupdocs.parser.options/language). |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


Ställer in det rektangulära området som begränsar sidområdet som används för textigenkänning.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Rektangeln, eller  null  för att skanna hela sidan. |
|

### setHandler(OcrEventHandler handler) {#setHandler-com.groupdocs.parser.options.OcrEventHandler-}
```
public void setHandler(OcrEventHandler handler)
```


Ställer in händelsehanteraren för att fånga OCR‑händelser.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Händelsehanteraren. |
|

### setUseSpellChecker(boolean useSpellChecker) {#setUseSpellChecker-boolean-}
```
public void setUseSpellChecker(boolean useSpellChecker)
```


Ställer in värdet som indikerar om stavningskontrollen används.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | useSpellChecker | boolean | true  för att aktivera stavningskontroll. |
|

