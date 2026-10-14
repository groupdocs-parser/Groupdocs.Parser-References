---
title: "PageTextArea"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente une zone de texte de page utilisée pour représenter une valeur de texte dans la fonctionnalité d'analyse par modèle ou d'analyse de formulaire."
type: docs
weight: 24
url: /fr/java/com.groupdocs.parser.data/pagetextarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTextArea extends PageArea
```

Représente une zone de texte de page utilisée pour représenter une valeur de texte dans la fonctionnalité d'analyse par modèle ou d'analyse de formulaire.

Une instance de la classe [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) est utilisée comme valeur de retour des méthodes suivantes :

* [Parser.getTextAreas()](../../com.groupdocs.parser/parser#getTextAreas--)
* [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-)
* [Parser.getTextAreas(int)](../../com.groupdocs.parser/parser#getTextAreas-int-)
* [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-)

De même, une instance de la classe [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) est utilisée comme valeur de la propriété [PageArea](../../com.groupdocs.parser.data/pagearea).
\*

Voir les exemples d'utilisation là-bas.

La zone de texte peut être simple ou composite. Dans le premier cas, elle contient un texte limité par une zone rectangulaire.
Dans le second cas, elle contient d'autres zones de texte ; les propriétés de texte et de tableau sont calculées à partir des zones de texte enfants.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [PageTextArea(String text, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initialise une nouvelle instance de la classe [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
|  | [PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initialise une nouvelle instance de la classe [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
|  | [PageTextArea(Iterable<PageTextArea> areas, Page page)](#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-) | Initialise une nouvelle instance de la classe [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getText()](#getText--) | Obtient le texte. |
|
|  | [getBaseLine()](#getBaseLine--) | Obtient la ligne de base. |
|
|  | [getTextStyle()](#getTextStyle--) | Obtient le style du texte tel que la taille de police, le nom de police, etc. |
|
|  | [getAreas()](#getAreas--) | Obtient la collection des zones de texte enfants. |
|
### PageTextArea(String text, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Page page, Rectangle rectangle)
```


Initialise une nouvelle instance de la classe [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | texte | java.lang.String | La valeur du texte. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | La page qui contient la zone de texte. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | La zone rectangulaire qui contient la zone de texte. |
|

### PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)
```


Initialise une nouvelle instance de la classe [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | texte | java.lang.String | La valeur du texte. |
|
|  | baseLine | java.lang.Double | La ligne de base du texte. |
|
|  | textStyle | [TextStyle](../../com.groupdocs.parser.data/textstyle) | Le style du texte. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | La page qui contient la zone de texte. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | La zone rectangulaire qui contient la zone de texte. |
|

### PageTextArea(Iterable<PageTextArea> areas, Page page) {#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-}
```
public PageTextArea(Iterable<PageTextArea> areas, Page page)
```


Initialise une nouvelle instance de la classe [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | zones | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | La collection des zones de texte de page enfants. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | La page qui contient la zone de texte. |
|

### getText() {#getText--}
```
public String getText()
```


Obtient le texte.


**Returns:**
java.lang.String - Une valeur de chaîne qui représente une valeur de la zone de texte de page.

### getBaseLine() {#getBaseLine--}
```
public double getBaseLine()
```


Obtient la ligne de base.


**Returns:**
double - Une valeur double qui représente la ligne de base.

### getTextStyle() {#getTextStyle--}
```
public TextStyle getTextStyle()
```


Obtient le style du texte tel que la taille de police, le nom de police, etc.


**Returns:**
[TextStyle](../../com.groupdocs.parser.data/textstyle) - An instance of [TextStyle](../../com.groupdocs.parser.data/textstyle) class that represents the text style.

### getAreas() {#getAreas--}
```
public List<PageTextArea> getAreas()
```


Obtient la collection des zones de texte enfants.


**Returns:**
java.util.List<com.groupdocs.parser.data.PageTextArea> - Une collection de zones de texte de page enfants ; vide si la zone de texte de page n'a pas d'enfants.

