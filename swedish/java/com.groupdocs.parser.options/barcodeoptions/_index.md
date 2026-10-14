---
title: "BarcodeOptions"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller de alternativ som används för streckkodsextraktion."
type: docs
weight: 10
url: /sv/java/com.groupdocs.parser.options/barcodeoptions/
---
**Inheritance:**
java.lang.Object
```
public class BarcodeOptions
```

Tillhandahåller de alternativ som används för streckkodsextraktion.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [BarcodeOptions()](#BarcodeOptions--) | Initierar en ny instans av klassen BarcodeOptions med standardvärden. |
|
|  | [BarcodeOptions(Rectangle rectangle)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-) | Initierar en ny instans av klassen BarcodeOptions med det rektangulära området. |
|
|  | [BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-) | Initierar en ny instans av klassen BarcodeOptions med kvalitetsinställningar och kodtyper. |
|
|  | [BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)](#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-) | Initierar en ny instans av klassen BarcodeOptions. |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [isAllowIncorrectBarcodes()](#isAllowIncorrectBarcodes--) | Hämtar värdet som indikerar om felaktiga streckkoder är tillåtna. |
|
|  | [getDimension()](#getDimension--) | Hämtar den minsta storleken på streckkodens minsta element. |
|
|  | [getImageQuality()](#getImageQuality--) | Hämtar kvaliteten på en källbild. |
|
|  | [getBarcodeQuality()](#getBarcodeQuality--) | Hämtar kvaliteten på en källstreckkod. |
|
|  | [getRectangle()](#getRectangle--) | Hämtar det rektangulära området som innehåller sidområden. |
|
|  | [getCodeTypes()](#getCodeTypes--) | Hämtar typerna av streckkoder som ska läsas. |
|
|  | [setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)](#setAllowIncorrectBarcodes-boolean-) | Ställer in värdet som indikerar om felaktiga streckkoder är tillåtna. |
|
|  | [setDimension(Float dimension)](#setDimension-java.lang.Float-) | Ställer in den minsta storleken på streckkodens minsta element. |
|
|  | [setImageQuality(QualityMode imageQuality)](#setImageQuality-com.groupdocs.parser.options.QualityMode-) | Ställer in kvaliteten på en källbild. |
|
|  | [setBarcodeQuality(QualityMode barcodeQuality)](#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-) | Ställer in kvaliteten på en källstreckkod. |
|
|  | [setRectangle(Rectangle rectangle)](#setRectangle-com.groupdocs.parser.data.Rectangle-) | Ställer in det rektangulära området som innehåller streckkoder. |
|
|  | [setCodeTypes(List<String> codeTypes)](#setCodeTypes-java.util.List-java.lang.String--) | Ställer in typerna av streckkoder som ska läsas. |
|
### BarcodeOptions() {#BarcodeOptions--}
```
public BarcodeOptions()
```


Initierar en ny instans av klassen BarcodeOptions med standardvärden.


### BarcodeOptions(Rectangle rectangle) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-}
```
public BarcodeOptions(Rectangle rectangle)
```


Initierar en ny instans av klassen BarcodeOptions med det rektangulära området.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området som innehåller streckkoder. |
|

### BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.String...-}
```
public BarcodeOptions(QualityMode imageQuality, QualityMode barcodeQuality, String[] codeTypes)
```


Initierar en ny instans av klassen BarcodeOptions med kvalitetsinställningar och kodtyper.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Kvaliteten på en källbild. |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Kvaliteten på en källstreckkod. |
|
|  | codeTypes | java.lang.String[] | Typerna av streckkoder som ska läsas. |
|

### BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes) {#BarcodeOptions-com.groupdocs.parser.data.Rectangle-com.groupdocs.parser.options.QualityMode-com.groupdocs.parser.options.QualityMode-java.lang.Float-boolean-java.lang.String...-}
```
public BarcodeOptions(Rectangle rectangle, QualityMode imageQuality, QualityMode barcodeQuality, Float dimension, boolean allowIncorrectBarcodes, String[] codeTypes)
```


Initierar en ny instans av klassen BarcodeOptions.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området som innehåller streckkoder. |
|
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Kvaliteten på en källbild. |
|
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Kvaliteten på en källstreckkod. |
|
|  | dimension | java.lang.Float | Den minsta storleken på streckkodens minsta element. |
|
|  | allowIncorrectBarcodes | boolean | Värdet som indikerar om felaktiga streckkoder är tillåtna. |
|
|  | codeTypes | java.lang.String[] | Typerna av streckkoder som ska läsas. |
|

### isAllowIncorrectBarcodes() {#isAllowIncorrectBarcodes--}
```
public boolean isAllowIncorrectBarcodes()
```


Hämtar värdet som indikerar om felaktiga streckkoder är tillåtna.


**Returns:**
boolean -  true  om felaktiga streckkoder är tillåtna; annars,  false .

### getDimension() {#getDimension--}
```
public Float getDimension()
```


Hämtar den minsta storleken på streckkodens minsta element.


**Returns:**
java.lang.Float - Det flyttalvärde som representerar streckkodens minsta element;  null  om auto mode används.

### getImageQuality() {#getImageQuality--}
```
public QualityMode getImageQuality()
```


Hämtar kvaliteten på en källbild.


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source image quality.

### getBarcodeQuality() {#getBarcodeQuality--}
```
public QualityMode getBarcodeQuality()
```


Hämtar kvaliteten på en källstreckkod.


**Returns:**
[QualityMode](../../com.groupdocs.parser.options/qualitymode) - The mode which defines the level of the source barcode quality.

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Hämtar det rektangulära området som innehåller sidområden.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains page areas;  null  if it isn't set.

### getCodeTypes() {#getCodeTypes--}
```
public List<String> getCodeTypes()
```


Hämtar typerna av streckkoder som ska läsas.


**Returns:**
java.util.List<java.lang.String> - Den skrivskyddade samlingen som innehåller typer av streckkoder att läsa; tom samling om den inte är inställd.

### setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes) {#setAllowIncorrectBarcodes-boolean-}
```
public void setAllowIncorrectBarcodes(boolean allowIncorrectBarcodes)
```


Ställer in värdet som indikerar om felaktiga streckkoder är tillåtna.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | allowIncorrectBarcodes | boolean | true  om felaktiga streckkoder är tillåtna. |
|

### setDimension(Float dimension) {#setDimension-java.lang.Float-}
```
public void setDimension(Float dimension)
```


Ställer in den minsta storleken på streckkodens minsta element.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | dimension | java.lang.Float | Streckkodens minsta element;  null  för auto mode. |
|

### setImageQuality(QualityMode imageQuality) {#setImageQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setImageQuality(QualityMode imageQuality)
```


Ställer in kvaliteten på en källbild.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | imageQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Bildkvalitetsläget. |
|

### setBarcodeQuality(QualityMode barcodeQuality) {#setBarcodeQuality-com.groupdocs.parser.options.QualityMode-}
```
public void setBarcodeQuality(QualityMode barcodeQuality)
```


Ställer in kvaliteten på en källstreckkod.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | barcodeQuality | [QualityMode](../../com.groupdocs.parser.options/qualitymode) | Streckkodskvalitetsläget. |
|

### setRectangle(Rectangle rectangle) {#setRectangle-com.groupdocs.parser.data.Rectangle-}
```
public void setRectangle(Rectangle rectangle)
```


Ställer in det rektangulära området som innehåller streckkoder.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området;  null  för att skanna hela sidan. |
|

### setCodeTypes(List<String> codeTypes) {#setCodeTypes-java.util.List-java.lang.String--}
```
public void setCodeTypes(List<String> codeTypes)
```


Ställer in typerna av streckkoder som ska läsas.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | codeTypes | java.util.List<java.lang.String> | Typerna av streckkoder;  null  eller tomt för alla typer. |
|

