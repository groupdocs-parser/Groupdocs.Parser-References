---
title: "OcrOptions"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit les options utilisées pour le connecteur OCR."
type: docs
weight: 27
url: /fr/java/com.groupdocs.parser.options/ocroptions/
---
**Inheritance:**
java.lang.Object
```
public class OcrOptions
```

Fournit les options utilisées pour le connecteur OCR.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [OcrOptions()](#OcrOptions--) | Initialise une nouvelle instance de la classe [OcrOptions](../../com.groupdocs.parser.options/ocroptions) avec les valeurs par défaut. |
|
|  | [OcrOptions(Rectangle rectangle)](#OcrOptions-com.groupdocs.parser.data.Rectangle-) | Initialise une nouvelle instance de la classe [OcrOptions](../../com.groupdocs.parser.options/ocroptions) avec une zone rectangulaire. |
|
|  | [OcrOptions(PagePreviewOptions pagePreviewOptions)](#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-) | Initialise une nouvelle instance de la classe [OcrOptions](../../com.groupdocs.parser.options/ocroptions) avec les options d'aperçu de page. |
|
|  | [OcrOptions(OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-) | Initialise une nouvelle instance de la classe [OcrOptions](../../com.groupdocs.parser.options/ocroptions) avec l'objet [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler). |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-) | Initialise une nouvelle instance de la classe [OcrOptions](../../com.groupdocs.parser.options/ocroptions) avec une zone rectangulaire et l'objet [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler). |
|
|  | [OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)](#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-) | Initialise une nouvelle instance de la classe [OcrOptions](../../com.groupdocs.parser.options/ocroptions). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Obtient la zone rectangulaire qui contraint la zone de la page utilisée pour la reconnaissance de texte. |
|
|  | [getHandler()](#getHandler--) | Obtient le gestionnaire d'événements pour capturer les événements OCR. |
|
|  | [getUseSpellChecker()](#getUseSpellChecker--) | Obtient la valeur indiquant si le correcteur orthographique est utilisé. |
|
|  | [getPagePreviewOptions()](#getPagePreviewOptions--) | Obtient les options d'aperçu de page utilisées pour rendre la page fournie au moteur OCR. |
|
|  | [setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)](#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-) | Définit les options d'aperçu de page utilisées pour rendre la page fournie au moteur OCR. |
|
|  | [getLanguage()](#getLanguage--) | Obtient la langue utilisée pour la reconnaissance optique de caractères. |
|
|  | [setLanguage(Language language)](#setLanguage-com.groupdocs.parser.options.Language-) | Définit la langue utilisée pour la reconnaissance optique de caractères. |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | Définit la zone rectangulaire qui contraint la zone de la page utilisée pour la reconnaissance de texte. |
|
|  | [setHandler(OcrEventHandler handler)](#setHandler-com.groupdocs.parser.options.OcrEventHandler-) | Définit le gestionnaire d'événements pour capturer les événements OCR. |
|
|  | [setUseSpellChecker(boolean useSpellChecker)](#setUseSpellChecker-boolean-) | Définit la valeur indiquant si le correcteur orthographique est utilisé. |
|
### OcrOptions() {#OcrOptions--}
```
public OcrOptions()
```


Initialise une nouvelle instance de la classe [OcrOptions](../../com.groupdocs.parser.options/ocroptions) avec les valeurs par défaut.


### OcrOptions(Rectangle rectangle) {#OcrOptions-com.groupdocs.parser.data.Rectangle-}
```
public OcrOptions(Rectangle rectangle)
```


Initialise une nouvelle instance de la classe [OcrOptions](../../com.groupdocs.parser.options/ocroptions) avec une zone rectangulaire.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | La zone rectangulaire qui contraint la zone de la page utilisée pour la reconnaissance de texte. |
|

### OcrOptions(PagePreviewOptions pagePreviewOptions) {#OcrOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public OcrOptions(PagePreviewOptions pagePreviewOptions)
```


Initialise une nouvelle instance de la classe [OcrOptions](../../com.groupdocs.parser.options/ocroptions) avec les options d'aperçu de page.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | Les options utilisées pour rendre l'aperçu de page fourni au moteur OCR. |
|

### OcrOptions(OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(OcrEventHandler handler)
```


Initialise une nouvelle instance de la classe [OcrOptions](../../com.groupdocs.parser.options/ocroptions) avec l'objet [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Une instance de [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) pour capturer les événements OCR. |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler)
```


Initialise une nouvelle instance de la classe [OcrOptions](../../com.groupdocs.parser.options/ocroptions) avec une zone rectangulaire et l'objet [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | La zone rectangulaire qui contraint la zone de la page utilisée pour la reconnaissance de texte. |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Une instance de [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) pour capturer les événements OCR. |
|

### OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker) {#OcrOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.OcrEventHandler-boolean-}
```
public OcrOptions(Rectangle rectangle, OcrEventHandler handler, boolean useSpellCheker)
```


Initialise une nouvelle instance de la classe [OcrOptions](../../com.groupdocs.parser.options/ocroptions).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | La zone rectangulaire qui contraint la zone de la page utilisée pour la reconnaissance de texte. |
|
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Une instance de [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) pour capturer les événements OCR. |
|
|  | useSpellCheker | boolean | La valeur indiquant si le correcteur orthographique est utilisé. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Obtient la zone rectangulaire qui contraint la zone de la page utilisée pour la reconnaissance de texte.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that constraints the page area which is used for text recognizing;  null  if it isn't set.

### getHandler() {#getHandler--}
```
public OcrEventHandler getHandler()
```


Obtient le gestionnaire d'événements pour capturer les événements OCR.


**Returns:**
[OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) - An instance of [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) class which is used to catch OCR events.

### getUseSpellChecker() {#getUseSpellChecker--}
```
public boolean getUseSpellChecker()
```


Obtient la valeur indiquant si le correcteur orthographique est utilisé.


**Returns:**
booléen -  true  si le correcteur orthographique est utilisé ; sinon,  false .

### getPagePreviewOptions() {#getPagePreviewOptions--}
```
public PagePreviewOptions getPagePreviewOptions()
```


Obtient les options d'aperçu de page utilisées pour rendre la page fournie au moteur OCR.


**Returns:**
[PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) - The [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions), or  null  if not set.

### setPagePreviewOptions(PagePreviewOptions pagePreviewOptions) {#setPagePreviewOptions-com.groupdocs.parser.options.PagePreviewOptions-}
```
public void setPagePreviewOptions(PagePreviewOptions pagePreviewOptions)
```


Définit les options d'aperçu de page utilisées pour rendre la page fournie au moteur OCR.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | pagePreviewOptions | [PagePreviewOptions](../../com.groupdocs.parser.options/pagepreviewoptions) | Les options d'aperçu de page. |
|

### getLanguage() {#getLanguage--}
```
public Language getLanguage()
```


Obtient la langue utilisée pour la reconnaissance optique de caractères.


**Returns:**
[Language](../../com.groupdocs.parser.options/language) - The [Language](../../com.groupdocs.parser.options/language) enum value. Defaults to [Language.Eng](../../com.groupdocs.parser.options/language#Eng).

### setLanguage(Language language) {#setLanguage-com.groupdocs.parser.options.Language-}
```
public void setLanguage(Language language)
```


Définit la langue utilisée pour la reconnaissance optique de caractères.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | language | [Language](../../com.groupdocs.parser.options/language) | La valeur d'énumération [Language](../../com.groupdocs.parser.options/language). |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


Définit la zone rectangulaire qui contraint la zone de la page utilisée pour la reconnaissance de texte.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Le rectangle, ou  null  pour analyser toute la page. |
|

### setHandler(OcrEventHandler handler) {#setHandler-com.groupdocs.parser.options.OcrEventHandler-}
```
public void setHandler(OcrEventHandler handler)
```


Définit le gestionnaire d'événements pour capturer les événements OCR.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | handler | [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler) | Le gestionnaire d'événements. |
|

### setUseSpellChecker(boolean useSpellChecker) {#setUseSpellChecker-boolean-}
```
public void setUseSpellChecker(boolean useSpellChecker)
```


Définit la valeur indiquant si le correcteur orthographique est utilisé.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | useSpellChecker | boolean | true  pour activer la vérification orthographique. |
|

