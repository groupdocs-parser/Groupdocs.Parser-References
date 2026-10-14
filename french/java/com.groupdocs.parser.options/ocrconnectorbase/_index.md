---
title: "OcrConnectorBase"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit la fonctionnalité OCR."
type: docs
weight: 25
url: /fr/java/com.groupdocs.parser.options/ocrconnectorbase/
---
**Inheritance:**
java.lang.Object
```
public class OcrConnectorBase
```

Fournit la fonctionnalité OCR.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [OcrConnectorBase()](#OcrConnectorBase--) | Initialise une nouvelle instance de la classe [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [isTextSupported()](#isTextSupported--) | Obtient la valeur qui indique si l'extraction de texte est prise en charge. |
|
|  | [isTextAreasSupported()](#isTextAreasSupported--) | Obtient la valeur qui indique si l'extraction des zones de texte est prise en charge. |
|
|  | [recognizeText(InputStream imageStream, OcrOptions options)](#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-) | Reconnaît un texte à partir du flux  imageStream . |
|
|  | [recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)](#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-) | Reconnaît les zones de texte à partir du flux  imageStream . |
|
### OcrConnectorBase() {#OcrConnectorBase--}
```
public OcrConnectorBase()
```


Initialise une nouvelle instance de la classe [OcrConnectorBase](../../com.groupdocs.parser.options/ocrconnectorbase).


### isTextSupported() {#isTextSupported--}
```
public boolean isTextSupported()
```


Obtient la valeur qui indique si l'extraction de texte est prise en charge.


**Returns:**
booléen -  true  si l'extraction de texte est prise en charge ; sinon,  false .

### isTextAreasSupported() {#isTextAreasSupported--}
```
public boolean isTextAreasSupported()
```


Obtient la valeur qui indique si l'extraction des zones de texte est prise en charge.


**Returns:**
booléen -  true  si les zones d'extraction de texte sont prises en charge ; sinon,  false .

### recognizeText(InputStream imageStream, OcrOptions options) {#recognizeText-java.io.InputStream-com.groupdocs.parser.options.OcrOptions-}
```
public String recognizeText(InputStream imageStream, OcrOptions options)
```


Reconnaît un texte à partir du flux  imageStream .


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | La représentation image de la page du document. |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Les options OCR. |
|

**Returns:**
java.lang.String - Une chaîne qui représente un texte reconnu ;  null  si la reconnaissance de texte n'est pas prise en charge.

### recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options) {#recognizeTextAreas-java.io.InputStream-com.groupdocs.parser.data.Size-com.groupdocs.parser.options.OcrOptions-}
```
public Iterable<PageTextArea> recognizeTextAreas(InputStream imageStream, Size pageSize, OcrOptions options)
```


Reconnaît les zones de texte à partir du flux  imageStream .


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | imageStream | java.io.InputStream | La représentation image de la page du document. |
|
|  | pageSize | [Size](../../com.groupdocs.parser.data/size) | La taille de la page du document. |
|
|  | options | [OcrOptions](../../com.groupdocs.parser.options/ocroptions) | Les options OCR. |
|

**Returns:**
java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> - Une collection d'objets [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) ;  null  si la reconnaissance des zones de texte n'est pas prise en charge.

