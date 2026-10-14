---
title: "OcrOptions"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die Optionen bereit, die für den OCR-Connector verwendet werden."
type: docs
weight: 27
url: /de/java/com.groupdocs.parser.options/ocroptions/
---
**Inheritance:**
java.lang.Object
```
public class OcrOptions
```

Stellt die Optionen bereit, die für den OCR-Connector verwendet werden.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [OcrOptions()](#OcrOptions--) | Initialisiert eine neue Instanz der Klasse [OcrOptions](../../com.groupdocs.parser.options/ocroptions) mit Standardwerten. |
|
|  | [OcrOptions(Rectangle rectangle)](#OcrOptions-com.groupdocs.parser.data.Rectangle-) | Initialisiert eine neue Instanz der Klasse [OcrOptions](../../com.groupdocs.parser.options/ocroptions) mit rechteckigem Bereich. |
|
|  | [OcrOptions(PagePreviewOptions pagePreviewOptions)](#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-) | Initialisiert eine neue Instanz der Klasse [OcrOptions](../../com.groupdocs.parser.options/ocroptions) mit Seitenvorschau‑Optionen. |
|
|  | [OcrOptions(OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-) | Initialisiert eine neue Instanz der Klasse [OcrOptions](../../com.groupdocs.parser.options/ocroptions) mit dem Objekt [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler). |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-) | Initialisiert eine neue Instanz der Klasse [OcrOptions](../../com.groupdocs.parser.options/ocroptions) mit rechteckigem Bereich und dem Objekt [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler). |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-) | Initialisiert eine neue Instanz der Klasse [OcrOptions](../../com.groupdocs.parser.options/ocroptions). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Gibt den rechteckigen Bereich zurück, der den Seitenbereich einschränkt, der für die Texterkennung verwendet wird. |
|
|  | [getHandler()](#getHandler--) | Gibt den Ereignishandler zurück, um OCR‑Ereignisse abzufangen. |
|
|  | [getUseSpellChecker()](#getUseSpellChecker--) | Liefert den Wert, der angibt, ob die Rechtschreibprüfung verwendet wird. |
|
|  | [getPagePreviewOptions()](#getPagePreviewOptions--) | Liefert die Seitenvorschau-Optionen, die zum Rendern der Seite verwendet werden, die an die OCR-Engine übergeben wird. |
|
|  | [setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)](#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-) | Legt die Seitenvorschau-Optionen fest, die zum Rendern der Seite verwendet werden, die an die OCR-Engine übergeben wird. |
|
|  | [getLanguage()](#getLanguage--) | Liefert die für die optische Zeichenerkennung verwendete Sprache. |
|
|  | [setLanguage(Language language)](#setLanguage-com.groupdocs.parser.options.Language-) | Legt die für die optische Zeichenerkennung verwendete Sprache fest. |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | Legt den rechteckigen Bereich fest, der den Seitenbereich einschränkt, der für die Texterkennung verwendet wird. |
|
|  | [setHandler(OcrEventHandler handler)](#setHandler-com.groupdocs.parser.options.OcrEventHandler-) | Legt den Ereignishandler fest, um OCR-Ereignisse abzufangen. |
|
|  | [setUseSpellChecker(boolean useSpellChecker)](#setUseSpellChecker-boolean-) | Legt den Wert fest, der angibt, ob die Rechtschreibprüfung verwendet wird. |
|
### OcrOptions() {#OcrOptions--}
```
public OcrOptions()
```


Initialisiert eine neue Instanz der Klasse [OcrOptions](../../com.groupdocs.parser.options/ocroptions) mit Standardwerten.


### OcrOptions(Rectangle rectangle) {#OcrOptions-com.groupdocs.parser.data.Rectangle-}
```
public OcrOptions(Rectangle rectangle)
```


Initialisiert eine neue Instanz der Klasse [OcrOptions](../../com.groupdocs.parser.options/ocroptions) mit rechteckigem Bereich.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Der rechteckige Bereich, der den Seitenbereich einschränkt, der für die Texterkennung verwendet wird. |
|

### OcrOptions(PagePreviewOptions pagePreviewOptions) {#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OcrOptions(PagePreviewOptions pagePreviewOptions)
```


Initialisiert eine neue Instanz der Klasse [OcrOptions](../../com.groupdocs.parser.options/ocroptions) mit Seitenvorschau‑Optionen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | Die Optionen, die zum Rendern der Seitenvorschau verwendet werden, die an die OCR-Engine übergeben wird. |
|

### OcrOptions(OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(OcrEventHandler handler)
```


Initialisiert eine neue Instanz der Klasse [OcrOptions](../../com.groupdocs.parser.options/ocroptions) mit dem Objekt [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Eine Instanz von [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler), um OCR-Ereignisse abzufangen. |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler)
```


Initialisiert eine neue Instanz der Klasse [OcrOptions](../../com.groupdocs.parser.options/ocroptions) mit rechteckigem Bereich und dem Objekt [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Der rechteckige Bereich, der den Seitenbereich einschränkt, der für die Texterkennung verwendet wird. |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Eine Instanz von [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler), um OCR-Ereignisse abzufangen. |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)
```


Initialisiert eine neue Instanz der Klasse [OcrOptions](../../com.groupdocs.parser.options/ocroptions).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Der rechteckige Bereich, der den Seitenbereich einschränkt, der für die Texterkennung verwendet wird. |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Eine Instanz von [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler), um OCR-Ereignisse abzufangen. |
|
|  | useSpellCheker | boolean | Der Wert, der angibt, ob die Rechtschreibprüfung verwendet wird. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Gibt den rechteckigen Bereich zurück, der den Seitenbereich einschränkt, der für die Texterkennung verwendet wird.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that constraints the page area which is used for text recognizing;  null  if it isn't set.

### getHandler() {#getHandler--}
```
public OcrEventHandler getHandler()
```


Gibt den Ereignishandler zurück, um OCR‑Ereignisse abzufangen.


**Returns:**
[OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) - An instance of [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) class which is used to catch OCR events.

### getUseSpellChecker() {#getUseSpellChecker--}
```
public boolean getUseSpellChecker()
```


Liefert den Wert, der angibt, ob die Rechtschreibprüfung verwendet wird.


**Returns:**
boolean -  true  wenn die Rechtschreibprüfung verwendet wird; andernfalls,  false .

### getPagePreviewOptions() {#getPagePreviewOptions--}
```
public PagePreviewOptions getPagePreviewOptions()
```


Liefert die Seitenvorschau-Optionen, die zum Rendern der Seite verwendet werden, die an die OCR-Engine übergeben wird.


**Returns:**
[PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) - The [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions), or  null  if not set.

### setPagePreviewOptions(PagePreviewOptions pagePreviewOptions) {#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public void setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)
```


Legt die Seitenvorschau-Optionen fest, die zum Rendern der Seite verwendet werden, die an die OCR-Engine übergeben wird.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | Die Seitenvorschau-Optionen. |
|

### getLanguage() {#getLanguage--}
```
public Language getLanguage()
```


Liefert die für die optische Zeichenerkennung verwendete Sprache.


**Returns:**
[Language](../../com.groupdocs.parser.options/language) - The [Language](../../com.groupdocs.parser.options/language) enum value. Defaults to [Language.Eng](../../com.groupdocs.parser.options/language#Eng).

### setLanguage(Language language) {#setLanguage-com.groupdocs.parser.options.Language-}
```
public void setLanguage(Language language)
```


Legt die für die optische Zeichenerkennung verwendete Sprache fest.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | language | [Language](../../com.groupdocs.parser.options/language) | Der [Language](../../com.groupdocs.parser.options/language)-Enum-Wert. |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


Legt den rechteckigen Bereich fest, der den Seitenbereich einschränkt, der für die Texterkennung verwendet wird.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Das Rechteck, oder  null  zum Scannen der gesamten Seite. |
|

### setHandler(OcrEventHandler handler) {#setHandler-com.groupdocs.parser.options.OcrEventHandler-}
```
public void setHandler(OcrEventHandler handler)
```


Legt den Ereignishandler fest, um OCR-Ereignisse abzufangen.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Der Ereignishandler. |
|

### setUseSpellChecker(boolean useSpellChecker) {#setUseSpellChecker-boolean-}
```
public void setUseSpellChecker(boolean useSpellChecker)
```


Legt den Wert fest, der angibt, ob die Rechtschreibprüfung verwendet wird.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | useSpellChecker | boolean | true  zum Aktivieren der Rechtschreibprüfung. |
|

