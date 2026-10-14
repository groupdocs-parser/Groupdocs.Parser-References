---
title: "Fonctionnalités"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente la liste des fonctionnalités prises en charge."
type: docs
weight: 18
url: /fr/java/com.groupdocs.parser.options/features/
---
**Inheritance:**
java.lang.Object
```
public abstract class Features
```

Représente la liste des fonctionnalités prises en charge. Permet d'obtenir des informations sur les fonctionnalités supportées ou non pour le document.

Une instance de cette classe est utilisée comme propriété [Parser.getFeatures()](../../com.groupdocs.parser/parser#getFeatures--) . Voir les exemples d'utilisation là-bas.

**Learn more:**

* [Get supported features](../https://docs.groupdocs.com/display/parserjava/Get+supported+features)

## Constructors

| Constructor | Description |
| --- | --- |
| [Features()](#Features--) |  |
## Methods

| Method | Description |
| --- | --- |
|  | [isFeatureSupported(String featureName)](#isFeatureSupported-java.lang.String-) | Renvoie la valeur indiquant si la fonctionnalité est prise en charge. |
|
|  | [isText()](#isText--) | Obtient la valeur indiquant si l'extraction de texte est prise en charge. |
|
|  | [isTextPage()](#isTextPage--) | Obtient la valeur indiquant si l'extraction de pages de texte est prise en charge. |
|
|  | [isFormattedText()](#isFormattedText--) | Obtient la valeur indiquant si l'extraction de texte formaté est prise en charge. |
|
|  | [isFormattedTextPage()](#isFormattedTextPage--) | Obtient la valeur indiquant si l'extraction de pages de texte formaté est prise en charge. |
|
|  | [isSearch()](#isSearch--) | Obtient la valeur indiquant si la recherche de texte est prise en charge. |
|
|  | [isHighlight()](#isHighlight--) | Obtient la valeur indiquant si l'extraction de surlignage est prise en charge. |
|
|  | [isBarcodes()](#isBarcodes--) | Obtient la valeur indiquant si l'extraction de codes-barres est prise en charge. |
|
|  | [isToc()](#isToc--) | Obtient la valeur indiquant si l'extraction de la table des matières est prise en charge. |
|
|  | [isMetadata()](#isMetadata--) | Obtient la valeur indiquant si l'extraction des métadonnées est prise en charge. |
|
|  | [isContainer()](#isContainer--) | Obtient la valeur indiquant si l'extraction du conteneur est prise en charge. |
|
|  | [isTextAreas()](#isTextAreas--) | Obtient la valeur indiquant si l'extraction des zones de texte est prise en charge. |
|
|  | [isStructure()](#isStructure--) | Obtient la valeur indiquant si l'extraction de la structure du texte est prise en charge. |
|
|  | [isImages()](#isImages--) | Obtient la valeur qui indique si l'extraction d'images est prise en charge. |
|
|  | [isHyperlinks()](#isHyperlinks--) | Obtient la valeur qui indique si l'extraction d'hyperliens est prise en charge. |
|
|  | [isTables()](#isTables--) | Obtient la valeur qui indique si l'extraction de tableaux est prise en charge. |
|
|  | [isAnnotations()](#isAnnotations--) | Obtient la valeur qui indique si l'extraction d'annotations est prise en charge. |
|
|  | [isParseByTemplate()](#isParseByTemplate--) | Obtient la valeur qui indique si l'analyse par modèle est prise en charge. |
|
|  | [isParseForm()](#isParseForm--) | Obtient la valeur qui indique si l'analyse de formulaires est prise en charge. |
|
|  | [isPreview()](#isPreview--) | Obtient la valeur qui indique si la génération d'aperçu est prise en charge. |
|
|  | [isPagePreview()](#isPagePreview--) | Obtient la valeur qui indique si la génération d'aperçu de page est prise en charge. |
|
|  | [isOcr()](#isOcr--) | Obtient la valeur qui indique si la fonctionnalité OCR est prise en charge. |
|
|  | [isWorksheet()](#isWorksheet--) | Obtient la valeur qui indique si l'extraction de la feuille de calcul est prise en charge. |
|
### Features() {#Features--}
```
public Features()
```


### isFeatureSupported(String featureName) {#isFeatureSupported-java.lang.String-}
```
public abstract boolean isFeatureSupported(String featureName)
```


Renvoie la valeur indiquant si la fonctionnalité est prise en charge.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | featureName | java.lang.String | Le nom de la fonctionnalité. |
|

**Returns:**
boolean -  true  si la fonctionnalité est prise en charge ; sinon,  false .

### isText() {#isText--}
```
public boolean isText()
```


Obtient la valeur indiquant si l'extraction de texte est prise en charge.


**Returns:**
boolean -  true  si l'extraction de texte est prise en charge ; sinon,  false .

### isTextPage() {#isTextPage--}
```
public boolean isTextPage()
```


Obtient la valeur indiquant si l'extraction de pages de texte est prise en charge.


**Returns:**
boolean -  true  si l'extraction de page de texte est prise en charge ; sinon,  false .

### isFormattedText() {#isFormattedText--}
```
public boolean isFormattedText()
```


Obtient la valeur indiquant si l'extraction de texte formaté est prise en charge.


**Returns:**
boolean -  true  si l'extraction de texte formaté est prise en charge ; sinon,  false .

### isFormattedTextPage() {#isFormattedTextPage--}
```
public boolean isFormattedTextPage()
```


Obtient la valeur indiquant si l'extraction de pages de texte formaté est prise en charge.


**Returns:**
boolean -  true  si la page de texte formaté est prise en charge ; sinon,  false .

### isSearch() {#isSearch--}
```
public boolean isSearch()
```


Obtient la valeur indiquant si la recherche de texte est prise en charge.


**Returns:**
boolean -  true  si la recherche de texte est prise en charge ; sinon,  false .

### isHighlight() {#isHighlight--}
```
public boolean isHighlight()
```


Obtient la valeur indiquant si l'extraction de surlignage est prise en charge.


**Returns:**
boolean -  true  si l'extraction de surlignage est prise en charge ; sinon,  false .

### isBarcodes() {#isBarcodes--}
```
public boolean isBarcodes()
```


Obtient la valeur indiquant si l'extraction de codes-barres est prise en charge.


**Returns:**
boolean -  true  si l'extraction de codes-barres est prise en charge ; sinon,  false .

### isToc() {#isToc--}
```
public boolean isToc()
```


Obtient la valeur indiquant si l'extraction de la table des matières est prise en charge.


**Returns:**
boolean -  true  si l'extraction de la table des matières est prise en charge ; sinon,  false .

### isMetadata() {#isMetadata--}
```
public boolean isMetadata()
```


Obtient la valeur indiquant si l'extraction des métadonnées est prise en charge.


**Returns:**
boolean -  true  si l'extraction des métadonnées est prise en charge ; sinon,  false .

### isContainer() {#isContainer--}
```
public boolean isContainer()
```


Obtient la valeur indiquant si l'extraction du conteneur est prise en charge.


**Returns:**
boolean -  true  si l'extraction de conteneur est prise en charge ; sinon,  false .

### isTextAreas() {#isTextAreas--}
```
public boolean isTextAreas()
```


Obtient la valeur indiquant si l'extraction des zones de texte est prise en charge.


**Returns:**
boolean -  true  si l'extraction de zones de texte est prise en charge ; sinon,  false .

### isStructure() {#isStructure--}
```
public boolean isStructure()
```


Obtient la valeur indiquant si l'extraction de la structure du texte est prise en charge.


**Returns:**
boolean -  true  si l'extraction de la structure du texte est prise en charge ; sinon,  false .

### isImages() {#isImages--}
```
public boolean isImages()
```


Obtient la valeur qui indique si l'extraction d'images est prise en charge.


**Returns:**
booléen -  true  si l'extraction d'images est prise en charge ; sinon,  false .

### isHyperlinks() {#isHyperlinks--}
```
public boolean isHyperlinks()
```


Obtient la valeur qui indique si l'extraction d'hyperliens est prise en charge.


**Returns:**
booléen -  true  si l'extraction d'hyperliens est prise en charge ; sinon,  false .

### isTables() {#isTables--}
```
public boolean isTables()
```


Obtient la valeur qui indique si l'extraction de tableaux est prise en charge.


**Returns:**
booléen -  true  si l'extraction de tableaux est prise en charge ; sinon,  false .

### isAnnotations() {#isAnnotations--}
```
public boolean isAnnotations()
```


Obtient la valeur qui indique si l'extraction d'annotations est prise en charge.


**Returns:**
booléen -  true  si l'extraction d'annotations est prise en charge ; sinon,  false .

### isParseByTemplate() {#isParseByTemplate--}
```
public boolean isParseByTemplate()
```


Obtient la valeur qui indique si l'analyse par modèle est prise en charge.


**Returns:**
booléen -  true  si l'analyse par modèle est prise en charge ; sinon,  false .

### isParseForm() {#isParseForm--}
```
public boolean isParseForm()
```


Obtient la valeur qui indique si l'analyse de formulaires est prise en charge.


**Returns:**
booléen -  true  si l'analyse de formulaire est prise en charge ; sinon,  false .

### isPreview() {#isPreview--}
```
public boolean isPreview()
```


Obtient la valeur qui indique si la génération d'aperçu est prise en charge.


**Returns:**
booléen -  true  si la génération d'aperçu est prise en charge ; sinon,  false .

### isPagePreview() {#isPagePreview--}
```
public boolean isPagePreview()
```


Obtient la valeur qui indique si la génération d'aperçu de page est prise en charge.


**Returns:**
booléen -  true  si la génération d'aperçu de page est prise en charge ; sinon,  false .

### isOcr() {#isOcr--}
```
public boolean isOcr()
```


Obtient la valeur qui indique si la fonctionnalité OCR est prise en charge.


**Returns:**
booléen -  true  si la fonctionnalité OCR est prise en charge ; sinon,  false .

### isWorksheet() {#isWorksheet--}
```
public boolean isWorksheet()
```


Obtient la valeur qui indique si l'extraction de la feuille de calcul est prise en charge.


**Returns:**
booléen -  true  si l'extraction de feuille de calcul est prise en charge ; sinon,  false .

