---
title: "TextOptions"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit les options utilisées pour l'extraction de texte."
type: docs
weight: 37
url: /fr/java/com.groupdocs.parser.options/textoptions/
---
**Inheritance:**
java.lang.Object
```
public class TextOptions
```

Fournit les options utilisées pour l'extraction de texte.

Une instance de la classe [TextOptions](../../com.groupdocs.parser.options/textoptions) est utilisée comme paramètre dans [Parser.getText(TextOptions)](../../com.groupdocs.parser/parser#getText-TextOptions-)
et les méthodes [Parser.getText(int, TextOptions)](../../com.groupdocs.parser/parser#getText-int--TextOptions-). Voir les exemples d'utilisation là-bas.

Il est utilisé pour spécifier le mode brut d'extraction de texte. Un texte dans ce mode est extrait de manière non précise
mais plus rapidement que dans le mode standard. Si le mode brut ne prend pas en charge le format du document,
alors ce paramètre est ignoré et le mode standard est utilisé.

**Learn more:**

* [Extract text in Raw Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Raw+mode)
* [Extract text in Accurate Mode](../https://docs.groupdocs.com/display/parserjava/Extract+text+in+Accurate+mode)

## Constructors

| Constructor | Description |
| --- | --- |
|  | [TextOptions(boolean useRawModeIfPossible)](#TextOptions-boolean-) | Initialise une nouvelle instance de la classe [TextOptions](../../com.groupdocs.parser.options/textoptions). |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr)](#TextOptions-boolean-boolean-) | Initialise une nouvelle instance de la classe [TextOptions](../../com.groupdocs.parser.options/textoptions) avec l'option d'utilisation de l'OCR. |
|
|  | [TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)](#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-) | Initialise une nouvelle instance de la classe [TextOptions](../../com.groupdocs.parser.options/textoptions) avec la possibilité de définir les options OCR. |
|
## Methods

| Method | Description |
| --- | --- |
|  | [isUseRawModeIfPossible()](#isUseRawModeIfPossible--) | Obtient la valeur qui indique si le mode brut est utilisé. |
|
|  | [isUseOcr()](#isUseOcr--) | Obtient la valeur qui indique si le connecteur OCR est utilisé pour extraire un texte. |
|
|  | [getOcrOptions()](#getOcrOptions--) | Obtient les options supplémentaires pour la fonctionnalité OCR. |
|
|  | [isIncludeAnnotations()](#isIncludeAnnotations--) | Obtient la valeur qui indique si les annotations sont incluses dans le texte extrait. |
|
|  | [setIncludeAnnotations(boolean includeAnnotations)](#setIncludeAnnotations-boolean-) | Définit la valeur qui indique si les annotations sont incluses dans le texte extrait. |
|
### TextOptions(boolean useRawModeIfPossible) {#TextOptions-boolean-}
```
public TextOptions(boolean useRawModeIfPossible)
```


Initialise une nouvelle instance de la classe [TextOptions](../../com.groupdocs.parser.options/textoptions).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | La valeur qui indique si le mode brut est utilisé. |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr) {#TextOptions-boolean-boolean-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr)
```


Initialise une nouvelle instance de la classe [TextOptions](../../com.groupdocs.parser.options/textoptions) avec l'option d'utilisation de l'OCR.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | La valeur qui indique si le mode brut est utilisé. |
|
|  | useOcr | boolean | La valeur qui indique si la fonctionnalité OCR est utilisée pour extraire un texte. |
|

### TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions) {#TextOptions-boolean-boolean-com.groupdocs.parser.options.OcrOptions-}
```
public TextOptions(boolean useRawModeIfPossible, boolean useOcr, OcrOptions ocrOptions)
```


Initialise une nouvelle instance de la classe [TextOptions](../../com.groupdocs.parser.options/textoptions) avec la possibilité de définir les options OCR.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | useRawModeIfPossible | boolean | La valeur qui indique si le mode brut est utilisé. |
|
|  | useOcr | boolean | La valeur qui indique si la fonctionnalité OCR est utilisée pour extraire un texte. |
|
|  | ocrOptions | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Les options supplémentaires pour la fonctionnalité OCR. |
|

### isUseRawModeIfPossible() {#isUseRawModeIfPossible--}
```
public boolean isUseRawModeIfPossible()
```


Obtient la valeur qui indique si le mode brut est utilisé.


**Returns:**
booléen -  true  si le mode brut est utilisé ; sinon,  false .

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

### isIncludeAnnotations() {#isIncludeAnnotations--}
```
public boolean isIncludeAnnotations()
```


Obtient la valeur qui indique si les annotations sont incluses dans le texte extrait. La valeur par défaut est  false .


**Returns:**
booléen -  true  si les annotations sont incluses ; sinon,  false .

### setIncludeAnnotations(boolean includeAnnotations) {#setIncludeAnnotations-boolean-}
```
public void setIncludeAnnotations(boolean includeAnnotations)
```


Définit la valeur qui indique si les annotations sont incluses dans le texte extrait.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | includeAnnotations | boolean | true  pour inclure les annotations dans le texte extrait. |
|

