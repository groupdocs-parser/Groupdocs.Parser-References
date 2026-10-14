---
title: "Funktionen"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt die Liste der unterstützten Funktionen dar."
type: docs
weight: 18
url: /de/java/com.groupdocs.parser.options/features/
---
**Inheritance:**
java.lang.Object
```
public abstract class Features
```

Stellt die Liste der unterstützten Funktionen dar. Ermöglicht das Abrufen von Informationen darüber, welche Funktionen für das Dokument unterstützt werden oder nicht.

Eine Instanz dieser Klasse wird als Eigenschaft [Parser.getFeatures()](../../com.groupdocs.parser/parser#getFeatures--) verwendet. Siehe dort die Anwendungsbeispiele.

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [Features()](#Features--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [isFeatureSupported(String featureName)](#isFeatureSupported-java.lang.String-) | Gibt den Wert zurück, der angibt, ob die Funktion unterstützt wird. |
|
|  | [isText()](#isText--) | Ermittelt den Wert, der angibt, ob die Textextraktion unterstützt wird. |
|
|  | [isTextPage()](#isTextPage--) | Ermittelt den Wert, der angibt, ob die Seiten-Textextraktion unterstützt wird. |
|
|  | [isFormattedText()](#isFormattedText--) | Ermittelt den Wert, der angibt, ob die formatierte Textextraktion unterstützt wird. |
|
|  | [isFormattedTextPage()](#isFormattedTextPage--) | Ermittelt den Wert, der angibt, ob die Extraktion formatierter Textseiten unterstützt wird. |
|
|  | [isSearch()](#isSearch--) | Ermittelt den Wert, der angibt, ob die Textsuche unterstützt wird. |
|
|  | [isHighlight()](#isHighlight--) | Ermittelt den Wert, der angibt, ob die Hervorhebungs‑Extraktion unterstützt wird. |
|
|  | [isBarcodes()](#isBarcodes--) | Ermittelt den Wert, der angibt, ob die Barcode‑Extraktion unterstützt wird. |
|
|  | [isToc()](#isToc--) | Ermittelt den Wert, der angibt, ob die Extraktion des Inhaltsverzeichnisses unterstützt wird. |
|
|  | [isMetadata()](#isMetadata--) | Ermittelt den Wert, der angibt, ob die Metadaten‑Extraktion unterstützt wird. |
|
|  | [isContainer()](#isContainer--) | Ermittelt den Wert, der angibt, ob die Container‑Extraktion unterstützt wird. |
|
|  | [isTextAreas()](#isTextAreas--) | Ermittelt den Wert, der angibt, ob die Extraktion von Textbereichen unterstützt wird. |
|
|  | [isStructure()](#isStructure--) | Ermittelt den Wert, der angibt, ob die Extraktion der Textstruktur unterstützt wird. |
|
|  | [isImages()](#isImages--) | Ermittelt den Wert, der angibt, ob die Bild‑Extraktion unterstützt wird. |
|
|  | [isHyperlinks()](#isHyperlinks--) | Ermittelt den Wert, der angibt, ob die Hyperlink‑Extraktion unterstützt wird. |
|
|  | [isTables()](#isTables--) | Ermittelt den Wert, der angibt, ob die Tabellen‑Extraktion unterstützt wird. |
|
|  | [isAnnotations()](#isAnnotations--) | Ermittelt den Wert, der angibt, ob die Annotations‑Extraktion unterstützt wird. |
|
|  | [isParseByTemplate()](#isParseByTemplate--) | Ermittelt den Wert, der angibt, ob das Parsen nach Vorlage unterstützt wird. |
|
|  | [isParseForm()](#isParseForm--) | Ermittelt den Wert, der angibt, ob das Formular‑Parsing unterstützt wird. |
|
|  | [isPreview()](#isPreview--) | Ermittelt den Wert, der angibt, ob die Vorschau‑Erstellung unterstützt wird. |
|
|  | [isPagePreview()](#isPagePreview--) | Ermittelt den Wert, der angibt, ob die Seitenvorschau‑Erstellung unterstützt wird. |
|
|  | [isOcr()](#isOcr--) | Ermittelt den Wert, der angibt, ob die OCR‑Funktionalität unterstützt wird. |
|
|  | [isWorksheet()](#isWorksheet--) | Ermittelt den Wert, der angibt, ob die Arbeitsblatt‑Extraktion unterstützt wird. |
|
### Features() {#Features--}
```
public Features()
```


### isFeatureSupported(String featureName) {#isFeatureSupported-java.lang.String-}
```
public abstract boolean isFeatureSupported(String featureName)
```


Gibt den Wert zurück, der angibt, ob die Funktion unterstützt wird.


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | featureName | java.lang.String | Der Funktionsname. |
|

**Returns:**
boolean -  true  wenn das Feature unterstützt wird; andernfalls,  false .

### isText() {#isText--}
```
public boolean isText()
```


Ermittelt den Wert, der angibt, ob die Textextraktion unterstützt wird.


**Returns:**
boolean -  true  wenn die Textextraktion unterstützt wird; andernfalls,  false .

### isTextPage() {#isTextPage--}
```
public boolean isTextPage()
```


Ermittelt den Wert, der angibt, ob die Seiten-Textextraktion unterstützt wird.


**Returns:**
boolean -  true  wenn die Textseiten‑Extraktion unterstützt wird; andernfalls,  false .

### isFormattedText() {#isFormattedText--}
```
public boolean isFormattedText()
```


Ermittelt den Wert, der angibt, ob die formatierte Textextraktion unterstützt wird.


**Returns:**
boolean -  true  wenn die formatierte Textextraktion unterstützt wird; andernfalls,  false .

### isFormattedTextPage() {#isFormattedTextPage--}
```
public boolean isFormattedTextPage()
```


Ermittelt den Wert, der angibt, ob die Extraktion formatierter Textseiten unterstützt wird.


**Returns:**
boolean -  true  wenn formatierte Textseite unterstützt wird; andernfalls  false .

### isSearch() {#isSearch--}
```
public boolean isSearch()
```


Ermittelt den Wert, der angibt, ob die Textsuche unterstützt wird.


**Returns:**
boolean -  true  wenn Textsuche unterstützt wird; andernfalls  false .

### isHighlight() {#isHighlight--}
```
public boolean isHighlight()
```


Ermittelt den Wert, der angibt, ob die Hervorhebungs‑Extraktion unterstützt wird.


**Returns:**
boolean -  true  wenn Hervorhebungs-Extraktion unterstützt wird; andernfalls  false .

### isBarcodes() {#isBarcodes--}
```
public boolean isBarcodes()
```


Ermittelt den Wert, der angibt, ob die Barcode‑Extraktion unterstützt wird.


**Returns:**
boolean -  true  wenn Barcode-Extraktion unterstützt wird; andernfalls  false .

### isToc() {#isToc--}
```
public boolean isToc()
```


Ermittelt den Wert, der angibt, ob die Extraktion des Inhaltsverzeichnisses unterstützt wird.


**Returns:**
boolean -  true  wenn Inhaltsverzeichnis-Extraktion unterstützt wird; andernfalls  false .

### isMetadata() {#isMetadata--}
```
public boolean isMetadata()
```


Ermittelt den Wert, der angibt, ob die Metadaten‑Extraktion unterstützt wird.


**Returns:**
boolean -  true  wenn Metadaten-Extraktion unterstützt wird; andernfalls  false .

### isContainer() {#isContainer--}
```
public boolean isContainer()
```


Ermittelt den Wert, der angibt, ob die Container‑Extraktion unterstützt wird.


**Returns:**
boolean -  true  wenn Container-Extraktion unterstützt wird; andernfalls  false .

### isTextAreas() {#isTextAreas--}
```
public boolean isTextAreas()
```


Ermittelt den Wert, der angibt, ob die Extraktion von Textbereichen unterstützt wird.


**Returns:**
boolean -  true  wenn Textbereichs-Extraktion unterstützt wird; andernfalls  false .

### isStructure() {#isStructure--}
```
public boolean isStructure()
```


Ermittelt den Wert, der angibt, ob die Extraktion der Textstruktur unterstützt wird.


**Returns:**
boolean -  true  wenn Textstruktur-Extraktion unterstützt wird; andernfalls  false .

### isImages() {#isImages--}
```
public boolean isImages()
```


Ermittelt den Wert, der angibt, ob die Bild‑Extraktion unterstützt wird.


**Returns:**
boolean -  true  wenn Bild-Extraktion unterstützt wird; andernfalls  false .

### isHyperlinks() {#isHyperlinks--}
```
public boolean isHyperlinks()
```


Ermittelt den Wert, der angibt, ob die Hyperlink‑Extraktion unterstützt wird.


**Returns:**
boolean -  true  wenn Hyperlink-Extraktion unterstützt wird; andernfalls  false .

### isTables() {#isTables--}
```
public boolean isTables()
```


Ermittelt den Wert, der angibt, ob die Tabellen‑Extraktion unterstützt wird.


**Returns:**
boolean -  true  wenn Tabellen-Extraktion unterstützt wird; andernfalls  false .

### isAnnotations() {#isAnnotations--}
```
public boolean isAnnotations()
```


Ermittelt den Wert, der angibt, ob die Annotations‑Extraktion unterstützt wird.


**Returns:**
boolean -  true  wenn Annotations-Extraktion unterstützt wird; andernfalls  false .

### isParseByTemplate() {#isParseByTemplate--}
```
public boolean isParseByTemplate()
```


Ermittelt den Wert, der angibt, ob das Parsen nach Vorlage unterstützt wird.


**Returns:**
boolean -  true  wenn das Parsen nach Vorlage unterstützt wird; andernfalls  false .

### isParseForm() {#isParseForm--}
```
public boolean isParseForm()
```


Ermittelt den Wert, der angibt, ob das Formular‑Parsing unterstützt wird.


**Returns:**
boolean -  true  wenn Formular-Parsing unterstützt wird; andernfalls  false .

### isPreview() {#isPreview--}
```
public boolean isPreview()
```


Ermittelt den Wert, der angibt, ob die Vorschau‑Erstellung unterstützt wird.


**Returns:**
boolean -  true  wenn Vorschaugenerierung unterstützt wird; andernfalls  false .

### isPagePreview() {#isPagePreview--}
```
public boolean isPagePreview()
```


Ermittelt den Wert, der angibt, ob die Seitenvorschau‑Erstellung unterstützt wird.


**Returns:**
boolean -  true  wenn die Seitenvorschaugenerierung unterstützt wird; andernfalls  false .

### isOcr() {#isOcr--}
```
public boolean isOcr()
```


Ermittelt den Wert, der angibt, ob die OCR‑Funktionalität unterstützt wird.


**Returns:**
boolean -  true  wenn OCR-Funktionalität unterstützt wird; andernfalls  false .

### isWorksheet() {#isWorksheet--}
```
public boolean isWorksheet()
```


Ermittelt den Wert, der angibt, ob die Arbeitsblatt‑Extraktion unterstützt wird.


**Returns:**
boolean -  true  wenn die Arbeitsblatt-Extraktion unterstützt wird; andernfalls  false .

