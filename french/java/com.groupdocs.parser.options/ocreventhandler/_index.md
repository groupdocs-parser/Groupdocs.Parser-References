---
title: "OcrEventHandler"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Fournit un gestionnaire pour les événements OCR."
type: docs
weight: 26
url: /fr/java/com.groupdocs.parser.options/ocreventhandler/
---
**Inheritance:**
java.lang.Object
```
public class OcrEventHandler
```

Fournit un gestionnaire pour les événements OCR.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [OcrEventHandler()](#OcrEventHandler--) | Initialise une nouvelle instance de la classe [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getWarnings()](#getWarnings--) | Obtient une liste de messages d'avertissement. |
|
|  | [hasWarnings()](#hasWarnings--) | Obtient la valeur qui indique si la liste des avertissements n'est pas vide. |
|
|  | [getWarnings(int pageIndex)](#getWarnings-int-) | Renvoie une liste de messages d'avertissement pour la page avec  pageIndex . |
|
|  | [onWarnings(int pageIndex, Iterable<String> warnings)](#onWarnings-int-java.lang.Iterable-java.lang.String--) | Définit les messages d'avertissement pour la page. |
|
### OcrEventHandler() {#OcrEventHandler--}
```
public OcrEventHandler()
```


Initialise une nouvelle instance de la classe [OcrEventHandler](../../com.groupdocs.parser.options/ocreventhandler).


### getWarnings() {#getWarnings--}
```
public List<String> getWarnings()
```


Obtient une liste de messages d'avertissement.


**Returns:**
java.util.List<java.lang.String> - Une liste de messages d'avertissement pour toutes les pages.

### hasWarnings() {#hasWarnings--}
```
public boolean hasWarnings()
```


Obtient la valeur qui indique si la liste des avertissements n'est pas vide.


**Returns:**
boolean -  true  si la liste des avertissements n'est pas vide ; sinon,  false .

### getWarnings(int pageIndex) {#getWarnings-int-}
```
public List<String> getWarnings(int pageIndex)
```


Renvoie une liste de messages d'avertissement pour la page avec  pageIndex .


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | pageIndex | int | L'index de page basé sur zéro. |
|

**Returns:**
java.util.List<java.lang.String> - Une liste de messages d'avertissement pour la page ; liste vide s'il n'y a aucun message d'avertissement pour la page.

### onWarnings(int pageIndex, Iterable<String> warnings) {#onWarnings-int-java.lang.Iterable-java.lang.String--}
```
public void onWarnings(int pageIndex, Iterable<String> warnings)
```


Définit les messages d'avertissement pour la page.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | pageIndex | int | L'index de page basé sur zéro. |
|
|  | warnings | java.lang.Iterable<java.lang.String> | La liste des messages d'avertissement pour la page. |
|

