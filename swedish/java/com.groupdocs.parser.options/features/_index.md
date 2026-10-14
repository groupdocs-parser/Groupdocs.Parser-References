---
title: "Funktioner"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar listan över stödda funktioner."
type: docs
weight: 18
url: /sv/java/com.groupdocs.parser.options/features/
---
**Inheritance:**
java.lang.Object
```
public abstract class Features
```

Representerar listan över stödjade funktioner. Gör det möjligt att få information om vilka funktioner som stöds eller inte för dokumentet.

En instans av denna klass används som egenskapen [Parser.getFeatures()](../../com.groupdocs.parser/parser#getFeatures--). Se användningsexemplen där.

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [Features()](#Features--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [isFeatureSupported(String featureName)](#isFeatureSupported-java.lang.String-) | Returnerar värdet som indikerar om funktionen stöds. |
|
|  | [isText()](#isText--) | Hämtar värdet som indikerar om textutdragning stöds. |
|
|  | [isTextPage()](#isTextPage--) | Hämtar värdet som indikerar om sidutdragning av text stöds. |
|
|  | [isFormattedText()](#isFormattedText--) | Hämtar värdet som indikerar om formaterad textutdragning stöds. |
|
|  | [isFormattedTextPage()](#isFormattedTextPage--) | Hämtar värdet som indikerar om formaterad sidutdragning av text stöds. |
|
|  | [isSearch()](#isSearch--) | Hämtar värdet som indikerar om textsökning stöds. |
|
|  | [isHighlight()](#isHighlight--) | Hämtar värdet som indikerar om markeringsutdragning stöds. |
|
|  | [isBarcodes()](#isBarcodes--) | Hämtar värdet som indikerar om streckkodsutdragning stöds. |
|
|  | [isToc()](#isToc--) | Hämtar värdet som indikerar om utdragning av innehållsförteckning stöds. |
|
|  | [isMetadata()](#isMetadata--) | Hämtar värdet som indikerar om metadatautdragning stöds. |
|
|  | [isContainer()](#isContainer--) | Hämtar värdet som indikerar om containerutdragning stöds. |
|
|  | [isTextAreas()](#isTextAreas--) | Hämtar värdet som indikerar om extrahering av textområden stöds. |
|
|  | [isStructure()](#isStructure--) | Hämtar värdet som indikerar om extrahering av textstruktur stöds. |
|
|  | [isImages()](#isImages--) | Hämtar värdet som indikerar om extrahering av bilder stöds. |
|
|  | [isHyperlinks()](#isHyperlinks--) | Hämtar värdet som indikerar om extrahering av hyperlänkar stöds. |
|
|  | [isTables()](#isTables--) | Hämtar värdet som indikerar om extrahering av tabeller stöds. |
|
|  | [isAnnotations()](#isAnnotations--) | Hämtar värdet som indikerar om extrahering av annotationer stöds. |
|
|  | [isParseByTemplate()](#isParseByTemplate--) | Hämtar värdet som indikerar om parsning enligt mall stöds. |
|
|  | [isParseForm()](#isParseForm--) | Hämtar värdet som indikerar om formulärparsning stöds. |
|
|  | [isPreview()](#isPreview--) | Hämtar värdet som indikerar om generering av förhandsgranskning stöds. |
|
|  | [isPagePreview()](#isPagePreview--) | Hämtar värdet som indikerar om generering av sidförhandsgranskning stöds. |
|
|  | [isOcr()](#isOcr--) | Hämtar värdet som indikerar om OCR-funktionalitet stöds. |
|
|  | [isWorksheet()](#isWorksheet--) | Hämtar värdet som indikerar om extrahering av kalkylblad stöds. |
|
### Features() {#Features--}
```
public Features()
```


### isFeatureSupported(String featureName) {#isFeatureSupported-java.lang.String-}
```
public abstract boolean isFeatureSupported(String featureName)
```


Returnerar värdet som indikerar om funktionen stöds.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | featureName | java.lang.String | Funktionens namn. |
|

**Returns:**
boolean -  true  om funktionen stöds; annars,  false .

### isText() {#isText--}
```
public boolean isText()
```


Hämtar värdet som indikerar om textutdragning stöds.


**Returns:**
boolean -  true  om textutdragning stöds; annars,  false .

### isTextPage() {#isTextPage--}
```
public boolean isTextPage()
```


Hämtar värdet som indikerar om sidutdragning av text stöds.


**Returns:**
boolean -  true  om textsidutdragning stöds; annars,  false .

### isFormattedText() {#isFormattedText--}
```
public boolean isFormattedText()
```


Hämtar värdet som indikerar om formaterad textutdragning stöds.


**Returns:**
boolean -  true  om formaterad textutdragning stöds; annars,  false .

### isFormattedTextPage() {#isFormattedTextPage--}
```
public boolean isFormattedTextPage()
```


Hämtar värdet som indikerar om formaterad sidutdragning av text stöds.


**Returns:**
boolean -  true  om formaterad textsida stöds; annars,  false .

### isSearch() {#isSearch--}
```
public boolean isSearch()
```


Hämtar värdet som indikerar om textsökning stöds.


**Returns:**
boolean -  true  om textsökning stöds; annars,  false .

### isHighlight() {#isHighlight--}
```
public boolean isHighlight()
```


Hämtar värdet som indikerar om markeringsutdragning stöds.


**Returns:**
boolean -  true  om markeringsutdragning stöds; annars,  false .

### isBarcodes() {#isBarcodes--}
```
public boolean isBarcodes()
```


Hämtar värdet som indikerar om streckkodsutdragning stöds.


**Returns:**
boolean -  true  om streckkodsutdragning stöds; annars,  false .

### isToc() {#isToc--}
```
public boolean isToc()
```


Hämtar värdet som indikerar om utdragning av innehållsförteckning stöds.


**Returns:**
boolean -  true  om innehållsförteckningsutdragning stöds; annars,  false .

### isMetadata() {#isMetadata--}
```
public boolean isMetadata()
```


Hämtar värdet som indikerar om metadatautdragning stöds.


**Returns:**
boolean -  true  om metadatautdragning stöds; annars,  false .

### isContainer() {#isContainer--}
```
public boolean isContainer()
```


Hämtar värdet som indikerar om containerutdragning stöds.


**Returns:**
boolean -  true  om containerutdragning stöds; annars,  false .

### isTextAreas() {#isTextAreas--}
```
public boolean isTextAreas()
```


Hämtar värdet som indikerar om extrahering av textområden stöds.


**Returns:**
boolean -  true  om extrahering av textområden stöds; annars,  false .

### isStructure() {#isStructure--}
```
public boolean isStructure()
```


Hämtar värdet som indikerar om extrahering av textstruktur stöds.


**Returns:**
boolean -  true  om extrahering av textstruktur stöds; annars,  false .

### isImages() {#isImages--}
```
public boolean isImages()
```


Hämtar värdet som indikerar om extrahering av bilder stöds.


**Returns:**
boolean -  true  om extrahering av bilder stöds; annars,  false .

### isHyperlinks() {#isHyperlinks--}
```
public boolean isHyperlinks()
```


Hämtar värdet som indikerar om extrahering av hyperlänkar stöds.


**Returns:**
boolean -  true  om extrahering av hyperlänkar stöds; annars,  false .

### isTables() {#isTables--}
```
public boolean isTables()
```


Hämtar värdet som indikerar om extrahering av tabeller stöds.


**Returns:**
boolean -  true  om extrahering av tabeller stöds; annars,  false .

### isAnnotations() {#isAnnotations--}
```
public boolean isAnnotations()
```


Hämtar värdet som indikerar om extrahering av annotationer stöds.


**Returns:**
boolean -  true  om extrahering av annotationer stöds; annars,  false .

### isParseByTemplate() {#isParseByTemplate--}
```
public boolean isParseByTemplate()
```


Hämtar värdet som indikerar om parsning enligt mall stöds.


**Returns:**
boolean -  true  om parsning med mall stöds; annars,  false .

### isParseForm() {#isParseForm--}
```
public boolean isParseForm()
```


Hämtar värdet som indikerar om formulärparsning stöds.


**Returns:**
boolean -  true  om formulärparsning stöds; annars,  false .

### isPreview() {#isPreview--}
```
public boolean isPreview()
```


Hämtar värdet som indikerar om generering av förhandsgranskning stöds.


**Returns:**
boolean -  true  om generering av förhandsgranskning stöds; annars,  false .

### isPagePreview() {#isPagePreview--}
```
public boolean isPagePreview()
```


Hämtar värdet som indikerar om generering av sidförhandsgranskning stöds.


**Returns:**
boolean -  true  om generering av sidförhandsgranskning stöds; annars,  false .

### isOcr() {#isOcr--}
```
public boolean isOcr()
```


Hämtar värdet som indikerar om OCR-funktionalitet stöds.


**Returns:**
boolean -  true  om OCR-funktionalitet stöds; annars,  false .

### isWorksheet() {#isWorksheet--}
```
public boolean isWorksheet()
```


Hämtar värdet som indikerar om extrahering av kalkylblad stöds.


**Returns:**
boolean -  true  om extrahering av kalkylblad stöds; annars,  false .

