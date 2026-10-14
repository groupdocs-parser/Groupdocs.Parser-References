---
title: "HighlightItem"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente une mise en évidence d'une partie du texte généralement utilisée pour expliquer le contexte du texte trouvé dans la fonctionnalité de recherche."
type: docs
weight: 14
url: /fr/java/com.groupdocs.parser.data/highlightitem/
---
**Inheritance:**
java.lang.Object
```
public class HighlightItem
```

Représente une mise en évidence, une partie du texte généralement utilisée pour expliquer le contexte du texte trouvé dans la fonctionnalité de recherche.

Une instance de la classe [HighlightItem](../../com.groupdocs.parser.data/highlightitem) est utilisée comme valeur de retour de la méthode [Parser.getHighlight(int, boolean, com.groupdocs.parser.options.HighlightOptions)](../../com.groupdocs.parser/parser#getHighlight-int--boolean--com.groupdocs.parser.options.HighlightOptions-),
[SearchResult.getLeftHighlightItem()](../../com.groupdocs.parser.data/searchresult#getLeftHighlightItem--) and [SearchResult.getRightHighlightItem()](../../com.groupdocs.parser.data/searchresult#getRightHighlightItem--) properties. See the usage examples there.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [HighlightItem(int position, String text)](#HighlightItem-int-java.lang.String-) | Initialise une nouvelle instance de la classe [HighlightItem](../../com.groupdocs.parser.data/highlightitem). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getPosition()](#getPosition--) | Obtient la position dans le texte du document. |
|
|  | [getText()](#getText--) | Obtient le texte de la mise en évidence. |
|
### HighlightItem(int position, String text) {#HighlightItem-int-java.lang.String-}
```
public HighlightItem(int position, String text)
```


Initialise une nouvelle instance de la classe [HighlightItem](../../com.groupdocs.parser.data/highlightitem).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | position | int | La position dans le texte du document. |
|
|  | texte | java.lang.String | Le texte de la mise en évidence. |
|

### getPosition() {#getPosition--}
```
public int getPosition()
```


Obtient la position dans le texte du document.


**Returns:**
int - Un indice basé sur zéro de la position de départ de la mise en évidence.

### getText() {#getText--}
```
public String getText()
```


Obtient le texte de la mise en évidence.


**Returns:**
java.lang.String - Une valeur de chaîne qui représente le texte de la mise en évidence.

