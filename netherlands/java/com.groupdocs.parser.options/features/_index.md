---
title: "Functies"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Stelt de lijst met ondersteunde functies voor."
type: docs
weight: 18
url: /nl/java/com.groupdocs.parser.options/features/
---
**Inheritance:**
java.lang.Object
```
public abstract class Features
```

Stelt de lijst met ondersteunde functies voor. Hiermee kunt u informatie verkrijgen over welke functies wel of niet worden ondersteund voor het document.

Een instantie van deze klasse wordt gebruikt als eigenschap [Parser.getFeatures()](../../com.groupdocs.parser/parser#getFeatures--). Zie daar de gebruiksvoorbeelden.

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [Features()](#Features--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [isFeatureSupported(String featureName)](#isFeatureSupported-java.lang.String-) | Retourneert de waarde die aangeeft of de functie wordt ondersteund. |
|
|  | [isText()](#isText--) | Haalt de waarde op die aangeeft of tekstextractie wordt ondersteund. |
|
|  | [isTextPage()](#isTextPage--) | Haalt de waarde op die aangeeft of pagina-tekstextractie wordt ondersteund. |
|
|  | [isFormattedText()](#isFormattedText--) | Haalt de waarde op die aangeeft of opgemaakte tekstextractie wordt ondersteund. |
|
|  | [isFormattedTextPage()](#isFormattedTextPage--) | Haalt de waarde op die aangeeft of opgemaakte pagina-tekstextractie wordt ondersteund. |
|
|  | [isSearch()](#isSearch--) | Haalt de waarde op die aangeeft of tekst zoeken wordt ondersteund. |
|
|  | [isHighlight()](#isHighlight--) | Haalt de waarde op die aangeeft of markeringsextractie wordt ondersteund. |
|
|  | [isBarcodes()](#isBarcodes--) | Haalt de waarde op die aangeeft of barcode-extractie wordt ondersteund. |
|
|  | [isToc()](#isToc--) | Haalt de waarde op die aangeeft of inhoudsopgave-extractie wordt ondersteund. |
|
|  | [isMetadata()](#isMetadata--) | Haalt de waarde op die aangeeft of metadata-extractie wordt ondersteund. |
|
|  | [isContainer()](#isContainer--) | Haalt de waarde op die aangeeft of container-extractie wordt ondersteund. |
|
|  | [isTextAreas()](#isTextAreas--) | Haalt de waarde op die aangeeft of tekstgebied-extractie wordt ondersteund. |
|
|  | [isStructure()](#isStructure--) | Haalt de waarde op die aangeeft of tekststructuur-extractie wordt ondersteund. |
|
|  | [isImages()](#isImages--) | Haalt de waarde op die aangeeft of afbeelding-extractie wordt ondersteund. |
|
|  | [isHyperlinks()](#isHyperlinks--) | Haalt de waarde op die aangeeft of hyperlink-extractie wordt ondersteund. |
|
|  | [isTables()](#isTables--) | Haalt de waarde op die aangeeft of tabel-extractie wordt ondersteund. |
|
|  | [isAnnotations()](#isAnnotations--) | Haalt de waarde op die aangeeft of annotatie-extractie wordt ondersteund. |
|
|  | [isParseByTemplate()](#isParseByTemplate--) | Haalt de waarde op die aangeeft of parsing op basis van sjabloon wordt ondersteund. |
|
|  | [isParseForm()](#isParseForm--) | Haalt de waarde op die aangeeft of formulierparsing wordt ondersteund. |
|
|  | [isPreview()](#isPreview--) | Haalt de waarde op die aangeeft of previewgeneratie wordt ondersteund. |
|
|  | [isPagePreview()](#isPagePreview--) | Haalt de waarde op die aangeeft of de paginapreviewgeneratie wordt ondersteund. |
|
|  | [isOcr()](#isOcr--) | Haalt de waarde op die aangeeft of OCR-functionaliteit wordt ondersteund. |
|
|  | [isWorksheet()](#isWorksheet--) | Haalt de waarde op die aangeeft of werkbladextractie wordt ondersteund. |
|
### Features() {#Features--}
```
public Features()
```


### isFeatureSupported(String featureName) {#isFeatureSupported-java.lang.String-}
```
public abstract boolean isFeatureSupported(String featureName)
```


Retourneert de waarde die aangeeft of de functie wordt ondersteund.


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | featureName | java.lang.String | De functienaam. |
|

**Returns:**
boolean -  true  als de functie wordt ondersteund; anders,  false .

### isText() {#isText--}
```
public boolean isText()
```


Haalt de waarde op die aangeeft of tekstextractie wordt ondersteund.


**Returns:**
boolean -  true  als tekstextractie wordt ondersteund; anders,  false .

### isTextPage() {#isTextPage--}
```
public boolean isTextPage()
```


Haalt de waarde op die aangeeft of pagina-tekstextractie wordt ondersteund.


**Returns:**
boolean -  true  als tekstpagina-extractie wordt ondersteund; anders,  false .

### isFormattedText() {#isFormattedText--}
```
public boolean isFormattedText()
```


Haalt de waarde op die aangeeft of opgemaakte tekstextractie wordt ondersteund.


**Returns:**
boolean -  true  als opgemaakte tekstextractie wordt ondersteund; anders,  false .

### isFormattedTextPage() {#isFormattedTextPage--}
```
public boolean isFormattedTextPage()
```


Haalt de waarde op die aangeeft of opgemaakte pagina-tekstextractie wordt ondersteund.


**Returns:**
boolean -  true  als opgemaakte tekstpagina wordt ondersteund; anders,  false .

### isSearch() {#isSearch--}
```
public boolean isSearch()
```


Haalt de waarde op die aangeeft of tekst zoeken wordt ondersteund.


**Returns:**
boolean -  true  als tekst zoeken wordt ondersteund; anders,  false .

### isHighlight() {#isHighlight--}
```
public boolean isHighlight()
```


Haalt de waarde op die aangeeft of markeringsextractie wordt ondersteund.


**Returns:**
boolean -  true  als markeringsextractie wordt ondersteund; anders,  false .

### isBarcodes() {#isBarcodes--}
```
public boolean isBarcodes()
```


Haalt de waarde op die aangeeft of barcode-extractie wordt ondersteund.


**Returns:**
boolean -  true  als barcode-extractie wordt ondersteund; anders,  false .

### isToc() {#isToc--}
```
public boolean isToc()
```


Haalt de waarde op die aangeeft of inhoudsopgave-extractie wordt ondersteund.


**Returns:**
boolean -  true  als inhoudsopgave-extractie wordt ondersteund; anders,  false .

### isMetadata() {#isMetadata--}
```
public boolean isMetadata()
```


Haalt de waarde op die aangeeft of metadata-extractie wordt ondersteund.


**Returns:**
boolean -  true  als metadata-extractie wordt ondersteund; anders,  false .

### isContainer() {#isContainer--}
```
public boolean isContainer()
```


Haalt de waarde op die aangeeft of container-extractie wordt ondersteund.


**Returns:**
boolean -  true  als container-extractie wordt ondersteund; anders,  false .

### isTextAreas() {#isTextAreas--}
```
public boolean isTextAreas()
```


Haalt de waarde op die aangeeft of tekstgebied-extractie wordt ondersteund.


**Returns:**
boolean -  true  als tekstgebiedsextractie wordt ondersteund; anders,  false .

### isStructure() {#isStructure--}
```
public boolean isStructure()
```


Haalt de waarde op die aangeeft of tekststructuur-extractie wordt ondersteund.


**Returns:**
boolean -  true  als tekststructuur-extractie wordt ondersteund; anders,  false .

### isImages() {#isImages--}
```
public boolean isImages()
```


Haalt de waarde op die aangeeft of afbeelding-extractie wordt ondersteund.


**Returns:**
boolean -  true  als afbeeldingsextractie wordt ondersteund; anders,  false .

### isHyperlinks() {#isHyperlinks--}
```
public boolean isHyperlinks()
```


Haalt de waarde op die aangeeft of hyperlink-extractie wordt ondersteund.


**Returns:**
boolean -  true  als hyperlink-extractie wordt ondersteund; anders,  false .

### isTables() {#isTables--}
```
public boolean isTables()
```


Haalt de waarde op die aangeeft of tabel-extractie wordt ondersteund.


**Returns:**
boolean -  true  als tabel-extractie wordt ondersteund; anders,  false .

### isAnnotations() {#isAnnotations--}
```
public boolean isAnnotations()
```


Haalt de waarde op die aangeeft of annotatie-extractie wordt ondersteund.


**Returns:**
boolean -  true  als annotatie-extractie wordt ondersteund; anders,  false .

### isParseByTemplate() {#isParseByTemplate--}
```
public boolean isParseByTemplate()
```


Haalt de waarde op die aangeeft of parsing op basis van sjabloon wordt ondersteund.


**Returns:**
boolean -  true  als parseren op basis van sjabloon wordt ondersteund; anders,  false .

### isParseForm() {#isParseForm--}
```
public boolean isParseForm()
```


Haalt de waarde op die aangeeft of formulierparsing wordt ondersteund.


**Returns:**
boolean -  true  als formulierparsing wordt ondersteund; anders,  false .

### isPreview() {#isPreview--}
```
public boolean isPreview()
```


Haalt de waarde op die aangeeft of previewgeneratie wordt ondersteund.


**Returns:**
boolean -  true  als previewgeneratie wordt ondersteund; anders,  false .

### isPagePreview() {#isPagePreview--}
```
public boolean isPagePreview()
```


Haalt de waarde op die aangeeft of de paginapreviewgeneratie wordt ondersteund.


**Returns:**
boolean -  true  als de paginapreviewgeneratie wordt ondersteund; anders,  false .

### isOcr() {#isOcr--}
```
public boolean isOcr()
```


Haalt de waarde op die aangeeft of OCR-functionaliteit wordt ondersteund.


**Returns:**
boolean -  true  als OCR-functionaliteit wordt ondersteund; anders,  false .

### isWorksheet() {#isWorksheet--}
```
public boolean isWorksheet()
```


Haalt de waarde op die aangeeft of werkbladextractie wordt ondersteund.


**Returns:**
boolean -  true  als werkbladextractie wordt ondersteund; anders,  false .

