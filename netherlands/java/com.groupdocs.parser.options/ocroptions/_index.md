---
title: "OcrOptions"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt de opties die worden gebruikt voor OCR Connector."
type: docs
weight: 27
url: /nl/java/com.groupdocs.parser.options/ocroptions/
---
**Inheritance:**
java.lang.Object
```
public class OcrOptions
```

Biedt de opties die worden gebruikt voor OCR Connector.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [OcrOptions()](#OcrOptions--) | Initialiseert een nieuw exemplaar van de [OcrOptions](../../com.groupdocs.parser.options/ocroptions) klasse met standaardwaarden. |
|
|  | [OcrOptions(Rectangle rectangle)](#OcrOptions-com.groupdocs.parser.data.Rectangle-) | Initialiseert een nieuw exemplaar van de [OcrOptions](../../com.groupdocs.parser.options/ocroptions) klasse met een rechthoekig gebied. |
|
|  | [OcrOptions(PagePreviewOptions pagePreviewOptions)](#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-) | Initialiseert een nieuw exemplaar van de [OcrOptions](../../com.groupdocs.parser.options/ocroptions) klasse met pagina-voorbeeldopties. |
|
|  | [OcrOptions(OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-) | Initialiseert een nieuw exemplaar van de [OcrOptions](../../com.groupdocs.parser.options/ocroptions) klasse met een [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) object. |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-) | Initialiseert een nieuw exemplaar van de [OcrOptions](../../com.groupdocs.parser.options/ocroptions) klasse met een rechthoekig gebied en een [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) object. |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-) | Initialiseert een nieuw exemplaar van de [OcrOptions](../../com.groupdocs.parser.options/ocroptions) klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Haalt het rechthoekige gebied op dat de pagina‑gebied beperkt dat wordt gebruikt voor teksterkenning. |
|
|  | [getHandler()](#getHandler--) | Haalt de event‑handler op om OCR‑gebeurtenissen te vangen. |
|
|  | [getUseSpellChecker()](#getUseSpellChecker--) | Haalt de waarde op die aangeeft of de spellingscontrole wordt gebruikt. |
|
|  | [getPagePreviewOptions()](#getPagePreviewOptions--) | Haalt de pagina-preview-opties op die worden gebruikt om de pagina te renderen die aan de OCR-engine wordt gevoed. |
|
|  | [setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)](#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-) | Stelt de pagina-preview-opties in die worden gebruikt om de pagina te renderen die aan de OCR-engine wordt gevoed. |
|
|  | [getLanguage()](#getLanguage--) | Haalt de taal op die wordt gebruikt voor optische tekenherkenning. |
|
|  | [setLanguage(Language language)](#setLanguage-com.groupdocs.parser.options.Language-) | Stelt de taal in die wordt gebruikt voor optische tekenherkenning. |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | Stelt het rechthoekige gebied in dat het paginagedeelte beperkt dat wordt gebruikt voor teksterkenning. |
|
|  | [setHandler(OcrEventHandler handler)](#setHandler-com.groupdocs.parser.options.OcrEventHandler-) | Stelt de gebeurtenishandler in om OCR-gebeurtenissen op te vangen. |
|
|  | [setUseSpellChecker(boolean useSpellChecker)](#setUseSpellChecker-boolean-) | Stelt de waarde in die aangeeft of de spellingscontrole wordt gebruikt. |
|
### OcrOptions() {#OcrOptions--}
```
public OcrOptions()
```


Initialiseert een nieuw exemplaar van de [OcrOptions](../../com.groupdocs.parser.options/ocroptions) klasse met standaardwaarden.


### OcrOptions(Rectangle rectangle) {#OcrOptions-com.groupdocs.parser.data.Rectangle-}
```
public OcrOptions(Rectangle rectangle)
```


Initialiseert een nieuw exemplaar van de [OcrOptions](../../com.groupdocs.parser.options/ocroptions) klasse met een rechthoekig gebied.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied dat het paginagedeelte beperkt dat wordt gebruikt voor teksterkenning. |
|

### OcrOptions(PagePreviewOptions pagePreviewOptions) {#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OcrOptions(PagePreviewOptions pagePreviewOptions)
```


Initialiseert een nieuw exemplaar van de [OcrOptions](../../com.groupdocs.parser.options/ocroptions) klasse met pagina-voorbeeldopties.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | De opties die worden gebruikt om de pagina-preview te renderen die aan de OCR-engine wordt gevoed. |
|

### OcrOptions(OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(OcrEventHandler handler)
```


Initialiseert een nieuw exemplaar van de [OcrOptions](../../com.groupdocs.parser.options/ocroptions) klasse met een [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) object.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Een instantie van [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) om OCR-gebeurtenissen op te vangen. |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler)
```


Initialiseert een nieuw exemplaar van de [OcrOptions](../../com.groupdocs.parser.options/ocroptions) klasse met een rechthoekig gebied en een [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) object.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied dat het paginagedeelte beperkt dat wordt gebruikt voor teksterkenning. |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Een instantie van [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) om OCR-gebeurtenissen op te vangen. |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)
```


Initialiseert een nieuw exemplaar van de [OcrOptions](../../com.groupdocs.parser.options/ocroptions) klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied dat het paginagedeelte beperkt dat wordt gebruikt voor teksterkenning. |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Een instantie van [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) om OCR-gebeurtenissen op te vangen. |
|
|  | useSpellCheker | boolean | De waarde die aangeeft of de spellingscontrole wordt gebruikt. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Haalt het rechthoekige gebied op dat de pagina‑gebied beperkt dat wordt gebruikt voor teksterkenning.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that constraints the page area which is used for text recognizing;  null  if it isn't set.

### getHandler() {#getHandler--}
```
public OcrEventHandler getHandler()
```


Haalt de event‑handler op om OCR‑gebeurtenissen te vangen.


**Returns:**
[OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) - An instance of [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) class which is used to catch OCR events.

### getUseSpellChecker() {#getUseSpellChecker--}
```
public boolean getUseSpellChecker()
```


Haalt de waarde op die aangeeft of de spellingscontrole wordt gebruikt.


**Returns:**
boolean -  true  als de spellingscontrole wordt gebruikt; anders,  false .

### getPagePreviewOptions() {#getPagePreviewOptions--}
```
public PagePreviewOptions getPagePreviewOptions()
```


Haalt de pagina-preview-opties op die worden gebruikt om de pagina te renderen die aan de OCR-engine wordt gevoed.


**Returns:**
[PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) - The [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions), or  null  if not set.

### setPagePreviewOptions(PagePreviewOptions pagePreviewOptions) {#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public void setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)
```


Stelt de pagina-preview-opties in die worden gebruikt om de pagina te renderen die aan de OCR-engine wordt gevoed.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | De pagina-preview-opties. |
|

### getLanguage() {#getLanguage--}
```
public Language getLanguage()
```


Haalt de taal op die wordt gebruikt voor optische tekenherkenning.


**Returns:**
[Language](../../com.groupdocs.parser.options/language) - The [Language](../../com.groupdocs.parser.options/language) enum value. Defaults to [Language.Eng](../../com.groupdocs.parser.options/language#Eng).

### setLanguage(Language language) {#setLanguage-com.groupdocs.parser.options.Language-}
```
public void setLanguage(Language language)
```


Stelt de taal in die wordt gebruikt voor optische tekenherkenning.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | language | [Language](../../com.groupdocs.parser.options/language) | De [Language](../../com.groupdocs.parser.options/language) enum-waarde. |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


Stelt het rechthoekige gebied in dat het paginagedeelte beperkt dat wordt gebruikt voor teksterkenning.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoek, of  null  om de hele pagina te scannen. |
|

### setHandler(OcrEventHandler handler) {#setHandler-com.groupdocs.parser.options.OcrEventHandler-}
```
public void setHandler(OcrEventHandler handler)
```


Stelt de gebeurtenishandler in om OCR-gebeurtenissen op te vangen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | De gebeurtenishandler. |
|

### setUseSpellChecker(boolean useSpellChecker) {#setUseSpellChecker-boolean-}
```
public void setUseSpellChecker(boolean useSpellChecker)
```


Stelt de waarde in die aangeeft of de spellingscontrole wordt gebruikt.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | useSpellChecker | boolean | true  om spellingscontrole in te schakelen. |
|

