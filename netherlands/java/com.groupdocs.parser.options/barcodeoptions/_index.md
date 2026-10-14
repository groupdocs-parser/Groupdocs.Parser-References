---
title: "BarcodeOptions"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Biedt de opties die worden gebruikt voor barcode-extractie."
type: docs
weight: 10
url: /nl/java/com.groupdocs.parser.options/barcodeoptions/
---
**Inheritance:**
java.lang.Object
```
public class BarcodeOptions
```

Biedt de opties die worden gebruikt voor barcode-extractie.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [BarcodeOptions()](#BarcodeOptions--) | Initialiseert een nieuw exemplaar van de BarcodeOptions-klasse met standaardwaarden. |
|
|  | [BarcodeOptions(Rectangle rectangle)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-) | Initialiseert een nieuw exemplaar van de BarcodeOptions-klasse met het rechthoekige gebied. |
|
|  | [BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-) | Initialiseert een nieuw exemplaar van de BarcodeOptions-klasse met kwaliteitsinstellingen en code-typen. |
|
|  | [BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-) | Initialiseert een nieuw exemplaar van de BarcodeOptions-klasse. |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [isAllowIncorrectBarcodes()](#isAllowIncorrectBarcodes--) | Haalt de waarde op die aangeeft of onjuiste barcodes zijn toegestaan. |
|
|  | [getDimension()](#getDimension--) | Haalt de minimale grootte van het minimale barcode-element op. |
|
|  | [getImageQuality()](#getImageQuality--) | Haalt de kwaliteit van een bronafbeelding op. |
|
|  | [getBarcodeQuality()](#getBarcodeQuality--) | Haalt de kwaliteit van een bron-barcode op. |
|
|  | [getRectangle()](#getRectangle--) | Haalt het rechthoekige gebied op dat pagina‑gebieden bevat. |
|
|  | [getCodeTypes()](#getCodeTypes--) | Haalt de typen barcodes op die gelezen moeten worden. |
|
|  | [setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)](#setAllowIncorrectBarcodes-boolean-) | Stelt de waarde in die aangeeft of onjuiste barcodes zijn toegestaan. |
|
|  | [setDimension(Float dimension)](#setDimension-java.lang.Float-) | Stelt de minimale grootte van het minimale barcode-element in. |
|
|  | [setImageQuality(QualityMode imageQuality)](#setImageQuality-com.groupdocs.parser.options.QualityMode-) | Stelt de kwaliteit van een bronafbeelding in. |
|
|  | [setBarcodeQuality(QualityMode barcodeQuality)](#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-) | Stelt de kwaliteit van een bron-barcode in. |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | Stelt het rechthoekige gebied in dat barcodes bevat. |
|
|  | [setCodeTypes(List<String> codeTypes)](#setCodeTypes-java.util.List-java.lang.String--) | Stelt de typen barcodes in die gelezen moeten worden. |
|
### BarcodeOptions() {#BarcodeOptions--}
```
public BarcodeOptions()
```


Initialiseert een nieuw exemplaar van de BarcodeOptions-klasse met standaardwaarden.


### BarcodeOptions(Rectangle rectangle) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-}
```
public BarcodeOptions(Rectangle rectangle)
```


Initialiseert een nieuw exemplaar van de BarcodeOptions-klasse met het rechthoekige gebied.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied dat barcodes bevat. |
|

### BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-}
```
public BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)
```


Initialiseert een nieuw exemplaar van de BarcodeOptions-klasse met kwaliteitsinstellingen en code-typen.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | De kwaliteit van een bronafbeelding. |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | De kwaliteit van een bronbarcode. |
|
|  | codeTypes | java.lang.String[] | De typen barcodes om te lezen. |
|

### BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-}
```
public BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)
```


Initialiseert een nieuw exemplaar van de BarcodeOptions-klasse.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied dat barcodes bevat. |
|
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | De kwaliteit van een bronafbeelding. |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | De kwaliteit van een bronbarcode. |
|
|  | dimension | java.lang.Float | De minimale grootte van het minimale barcode‑element. |
|
|  | allowIncorrectBarcodes | boolean | De waarde die aangeeft of de onjuiste barcodes zijn toegestaan. |
|
|  | codeTypes | java.lang.String[] | De typen barcodes om te lezen. |
|

### isAllowIncorrectBarcodes() {#isAllowIncorrectBarcodes--}
```
public boolean isAllowIncorrectBarcodes()
```


Haalt de waarde op die aangeeft of onjuiste barcodes zijn toegestaan.


**Returns:**
boolean -  true  als de onjuiste barcodes zijn toegestaan; anders,  false .

### getDimension() {#getDimension--}
```
public Float getDimension()
```


Haalt de minimale grootte van het minimale barcode-element op.


**Returns:**
java.lang.Float - De float‑waarde die het minimale barcode‑element vertegenwoordigt;  null  als de automatische modus wordt gebruikt.

### getImageQuality() {#getImageQuality--}
```
public QualityMode getImageQuality()
```


Haalt de kwaliteit van een bronafbeelding op.


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source image quality.

### getBarcodeQuality() {#getBarcodeQuality--}
```
public QualityMode getBarcodeQuality()
```


Haalt de kwaliteit van een bron-barcode op.


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source barcode quality.

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Haalt het rechthoekige gebied op dat pagina‑gebieden bevat.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getCodeTypes() {#getCodeTypes--}
```
public List<String> getCodeTypes()
```


Haalt de typen barcodes op die gelezen moeten worden.


**Returns:**
java.util.List<java.lang.String> - De alleen‑lezen collectie die een typen barcodes bevat om te lezen; lege collectie als deze niet is ingesteld.

### setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes) {#setAllowIncorrectBarcodes-boolean-}
```
public void setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)
```


Stelt de waarde in die aangeeft of onjuiste barcodes zijn toegestaan.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | allowIncorrectBarcodes | boolean | true  als de onjuiste barcodes zijn toegestaan. |
|

### setDimension(Float dimension) {#setDimension-java.lang.Float-}
```
public void setDimension(Float dimension)
```


Stelt de minimale grootte van het minimale barcode-element in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | dimension | java.lang.Float | Het minimale barcode‑element;  null  voor automatische modus. |
|

### setImageQuality(QualityMode imageQuality) {#setImageQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setImageQuality(QualityMode imageQuality)
```


Stelt de kwaliteit van een bronafbeelding in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | De afbeeldingskwaliteitsmodus. |
|

### setBarcodeQuality(QualityMode barcodeQuality) {#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setBarcodeQuality(QualityMode barcodeQuality)
```


Stelt de kwaliteit van een bron-barcode in.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | De barcode‑kwaliteitsmodus. |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


Stelt het rechthoekige gebied in dat barcodes bevat.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied;  null  om de hele pagina te scannen. |
|

### setCodeTypes(List<String> codeTypes) {#setCodeTypes-java.util.List-java.lang.String--}
```
public void setCodeTypes(List<String> codeTypes)
```


Stelt de typen barcodes in die gelezen moeten worden.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | codeTypes | java.util.List<java.lang.String> | De typen barcodes;  null  of leeg voor alle typen. |
|

