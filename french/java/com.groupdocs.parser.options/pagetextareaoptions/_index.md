---
title: "PageTextAreaOptions"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit les options utilisées pour l'extraction des zones de texte de page."
type: docs
weight: 32
url: /fr/java/com.groupdocs.parser.options/pagetextareaoptions/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.options.PageAreaOptions](../../com.groupdocs.parser.options/pageareaoptions)
```
public class PageTextAreaOptions extends PageAreaOptions
```

Fournit les options utilisées pour l'extraction des zones de texte de page.

Une instance de la classe [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) est utilisée comme paramètre dans [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-)
et les méthodes [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-) . Consultez les exemples d'utilisation à cet endroit.

**Learn more:**

* [Extract text areas](../https://docs.groupdocs.com/display/parserjava/Extract+text+areas)

## Constructors

| Constructor | Description |
| --- | --- |
|  | [PageTextAreaOptions()](#PageTextAreaOptions--) | Initialise une nouvelle instance de la classe [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) avec les valeurs par défaut. |
|
|  | [PageTextAreaOptions(boolean useOcr)](#PageTextAreaOptions-boolean-) | Initialise une nouvelle instance de la classe [TextOptions](../../com.groupdocs.parser.options/textoptions) avec l'option d'utilisation de l'OCR. |
|
|  | [PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)](#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-) | Initialise une nouvelle instance de la classe [TextOptions](../../com.groupdocs.parser.options/textoptions) avec la possibilité de définir les options OCR. |
|
|  | [PageTextAreaOptions(String expression)](#PageTextAreaOptions-java.lang.String-) | Initialise une nouvelle instance de la classe [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) avec l'expression régulière. |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-) | Initialise une nouvelle instance de la classe [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) avec l'expression régulière et la zone rectangulaire. |
|
|  | [PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-) | Initialise une nouvelle instance de la classe [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) avec l'expression régulière, la zone rectangulaire et la taille de la bordure ignorée. |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-) | Initialise une nouvelle instance de la classe [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions). |
|
|  | [PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)](#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-) | Initialise une nouvelle instance de la classe [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) avec la taille de la bordure ignorée. |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getExpression()](#getExpression--) | Obtient l'expression régulière. |
|
|  | [isMatchCase()](#isMatchCase--) | Obtient la valeur qui indique si la casse du texte n'est pas ignorée. |
|
|  | [isUniteSegments()](#isUniteSegments--) | Obtient la valeur qui indique si les segments sont unis. |
|
|  | [isIgnoreFormatting()](#isIgnoreFormatting--) | Obtient la valeur qui indique si le formatage du texte est ignoré. |
|
|  | [isUseOcr()](#isUseOcr--) | Obtient la valeur qui indique si le connecteur OCR est utilisé pour extraire un texte. |
|
|  | [getOcrOptions()](#getOcrOptions--) | Obtient les options supplémentaires pour la fonctionnalité OCR. |
|
### PageTextAreaOptions() {#PageTextAreaOptions--}
```
public PageTextAreaOptions()
```


Initialise une nouvelle instance de la classe [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) avec les valeurs par défaut.


### PageTextAreaOptions(boolean useOcr) {#PageTextAreaOptions-boolean-}
```
public PageTextAreaOptions(boolean useOcr)
```


Initialise une nouvelle instance de la classe [TextOptions](../../com.groupdocs.parser.options/textoptions) avec l'option d'utilisation de l'OCR.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | useOcr | boolean | La valeur qui indique si la fonctionnalité OCR est utilisée pour extraire un texte. |
|

### PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions) {#PageTextAreaOptions-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public PageTextAreaOptions(boolean useOcr, OcrOptions ocrOptions)
```


Initialise une nouvelle instance de la classe [TextOptions](../../com.groupdocs.parser.options/textoptions) avec la possibilité de définir les options OCR.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | useOcr | boolean | La valeur qui indique si la fonctionnalité OCR est utilisée pour extraire un texte. |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Les options supplémentaires pour la fonctionnalité OCR. |
|

### PageTextAreaOptions(String expression) {#PageTextAreaOptions-java.lang.String-}
```
public PageTextAreaOptions(String expression)
```


Initialise une nouvelle instance de la classe [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) avec l'expression régulière. Les autres options sont définies par défaut (voir les remarques pour plus de détails).

Les propriétés suivantes ont des valeurs par défaut :

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 
* Rectangle:  null 


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | expression | java.lang.String | L'expression régulière. |
|

### PageTextAreaOptions(String expression, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle)
```


Initialise une nouvelle instance de la classe [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) avec l'expression régulière et la zone rectangulaire. Les autres options sont définies par défaut (voir les remarques pour plus de détails).

Les propriétés suivantes ont des valeurs par défaut :

* MatchCase:  false 
* UniteSegments:  false 
* IgnoreFormatting:  false 


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | expression | java.lang.String | L'expression régulière. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | La zone rectangulaire qui contient les zones de page. |
|

### PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, Rectangle rectangle, double rectangleTolerance)
```


Initialise une nouvelle instance de la classe [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) avec l'expression régulière, la zone rectangulaire et la taille de la bordure ignorée. Les autres options sont définies par défaut (voir les remarques pour plus de détails).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | expression | java.lang.String | L'expression régulière. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | La zone rectangulaire qui contient les zones de page. |
|
|  | rectangleTolerance | double | La taille de la bordure qui est ignorée lorsqu'elle est capturée par la zone rectangulaire. Elle est mesurée par la fraction de la hauteur d'un élément de texte. |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle)
```


Initialise une nouvelle instance de la classe [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | expression | java.lang.String | L'expression régulière. |
|
|  | matchCase | boolean | La valeur qui indique si la casse du texte n'est pas ignorée. |
|
|  | uniteSegments | boolean | La valeur qui indique si les segments sont unis. |
|
|  | ignoreFormatting | boolean | La valeur qui indique si le formatage du texte est ignoré. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | La zone rectangulaire qui contient les zones de page. |
|

### PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance) {#PageTextAreaOptions-java.lang.String-boolean-boolean-boolean-com.groupdocs.parser.data.Rectangle-double-}
```
public PageTextAreaOptions(String expression, boolean matchCase, boolean uniteSegments, boolean ignoreFormatting, Rectangle rectangle, double rectangleTolerance)
```


Initialise une nouvelle instance de la classe [PageTextAreaOptions](../../com.groupdocs.parser.options/pagetextareaoptions) avec la taille de la bordure ignorée.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | expression | java.lang.String | L'expression régulière. |
|
|  | matchCase | boolean | La valeur qui indique si la casse du texte n'est pas ignorée. |
|
|  | uniteSegments | boolean | La valeur qui indique si les segments sont unis. |
|
|  | ignoreFormatting | boolean | La valeur qui indique si le formatage du texte est ignoré. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | La zone rectangulaire qui contient les zones de page. |
|
|  | rectangleTolerance | double | La taille de la bordure qui est ignorée lorsqu'elle est capturée par la zone rectangulaire. Elle est mesurée par la fraction de la hauteur d'un élément de texte. |
|

### getExpression() {#getExpression--}
```
public String getExpression()
```


Obtient l'expression régulière.


**Returns:**
java.lang.String - Une chaîne qui représente l'expression régulière.

### isMatchCase() {#isMatchCase--}
```
public boolean isMatchCase()
```


Obtient la valeur qui indique si la casse du texte n'est pas ignorée.


**Returns:**
boolean -  true  si la casse du texte n'est pas ignorée ; sinon,  false .

### isUniteSegments() {#isUniteSegments--}
```
public boolean isUniteSegments()
```


Obtient la valeur qui indique si les segments sont unis.


**Returns:**
boolean - {code true} si les segments sont unis ; sinon, {code false}.

### isIgnoreFormatting() {#isIgnoreFormatting--}
```
public boolean isIgnoreFormatting()
```


Obtient la valeur qui indique si le formatage du texte est ignoré.


**Returns:**
boolean -  true  si le formatage du texte est ignoré ; sinon,  false .

### isUseOcr() {#isUseOcr--}
```
public boolean isUseOcr()
```


Obtient la valeur qui indique si le connecteur OCR est utilisé pour extraire un texte.


**Returns:**
booléen -  true  si la fonctionnalité OCR est utilisée ; sinon,  false .

### getOcrOptions() {#getOcrOptions--}
```
public OcrOptions getOcrOptions()
```


Obtient les options supplémentaires pour la fonctionnalité OCR.


**Returns:**
[OcrOptions](../../com.groupdocs.parser.options/ocroptions) - An instance of [OcrOptions](../../com.groupdocs.parser.options/ocroptions) class with the additional OCR options.

