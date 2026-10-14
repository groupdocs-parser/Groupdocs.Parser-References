---
title: "SearchResult"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente le résultat de la recherche dans la fonctionnalité de recherche."
type: docs
weight: 27
url: /fr/java/com.groupdocs.parser.data/searchresult/
---
**Inheritance:**
java.lang.Object
```
public class SearchResult
```

Représente le résultat de la recherche dans la fonctionnalité de recherche.

Une instance de la classe SearchResult est utilisée comme valeur de retour de [Parser.search(String)](../../com.groupdocs.parser/parser#search-String-).
et les méthodes [Parser.search(String, com.groupdocs.parser.options.SearchOptions)](../../com.groupdocs.parser/parser#search-String--com.groupdocs.parser.options.SearchOptions-). Voir les exemples d'utilisation là-bas.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)](#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-) | Initialise une nouvelle instance de la classe [SearchResult](../../com.groupdocs.parser.data/searchresult). |
|
|  | [SearchResult(int position, String text, Integer pageIndex)](#SearchResult-int-java.lang.String-java.lang.Integer-) | Initialise une nouvelle instance de la classe [SearchResult](../../com.groupdocs.parser.data/searchresult). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getPosition()](#getPosition--) | Obtient la position dans le texte du document. |
|
|  | [getText()](#getText--) | Obtient le texte. |
|
|  | [getPageIndex()](#getPageIndex--) | Obtient l'index de page où le texte est trouvé. |
|
|  | [getLeftHighlightItem()](#getLeftHighlightItem--) | Obtient la mise en évidence gauche. |
|
|  | [getRightHighlightItem()](#getRightHighlightItem--) | Obtient la mise en évidence droite. |
|
### SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem) {#SearchResult-int-java.lang.String-java.lang.Integer-com.groupdocs.parser.data.HighlightItem-com.groupdocs.parser.data.HighlightItem-}
```
public SearchResult(int position, String text, Integer pageIndex, HighlightItem leftHighlightItem, HighlightItem rightHighlightItem)
```


Initialise une nouvelle instance de la classe [SearchResult](../../com.groupdocs.parser.data/searchresult).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | position | int | La position dans le texte du document. |
|
|  | texte | java.lang.String | Le texte trouvé. |
|
|  | pageIndex | java.lang.Integer | L'index de page où le texte est trouvé. |
|
|  | leftHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | Le surlignage gauche. |
|
|  | rightHighlightItem | [HighlightItem](../../com.groupdocs.parser.data/highlightitem) | Le surlignage droit. |
|

### SearchResult(int position, String text, Integer pageIndex) {#SearchResult-int-java.lang.String-java.lang.Integer-}
```
public SearchResult(int position, String text, Integer pageIndex)
```


Initialise une nouvelle instance de la classe [SearchResult](../../com.groupdocs.parser.data/searchresult).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | position | int | La position dans le texte du document. |
|
|  | texte | java.lang.String | Le texte trouvé. |
|
|  | pageIndex | java.lang.Integer | L'index de page où le texte est trouvé. |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


Obtient la position dans le texte du document.


**Returns:**
int - Un indice basé sur zéro de la position de départ du résultat de recherche.

### getText() {#getText--}
```
public String getText()
```


Obtient le texte.


**Returns:**
java.lang.String - Une valeur de chaîne qui représente le texte trouvé.

### getPageIndex() {#getPageIndex--}
```
public Integer getPageIndex()
```


Obtient l'index de page où le texte est trouvé.


**Returns:**
java.lang.Integer - Un indice basé sur zéro de la page où le texte est trouvé ;  null  si la recherche est effectuée sur le texte complet du document.

### getLeftHighlightItem() {#getLeftHighlightItem--}
```
public HighlightItem getLeftHighlightItem()
```


Obtient la mise en évidence gauche.


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

### getRightHighlightItem() {#getRightHighlightItem--}
```
public HighlightItem getRightHighlightItem()
```


Obtient la mise en évidence droite.


**Returns:**
[HighlightItem](../../com.groupdocs.parser.data/highlightitem) - An instance of [HighlightItem](../../com.groupdocs.parser.data/highlightitem) class;  null  if it isn't set.

