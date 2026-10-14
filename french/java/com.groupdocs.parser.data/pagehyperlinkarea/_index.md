---
title: "PageHyperlinkArea"
second_title: "Référence API de GroupDocs.Parser for Java"
description: "Représente une zone de page utilisée pour représenter un hyperlien sur la page."
type: docs
weight: 20
url: /fr/java/com.groupdocs.parser.data/pagehyperlinkarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageHyperlinkArea extends PageArea
```

Représente une zone de page utilisée pour représenter un hyperlien sur la page.

Une instance de la classe [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) est utilisée comme valeur de retour des méthodes suivantes:

* [Parser.getHyperlinks()](../../com.groupdocs.parser/parser#getHyperlinks--)
* [Parser.getHyperlinks(PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-PageAreaOptions-)
* [Parser.getHyperlinks(int)](../../com.groupdocs.parser/parser#getHyperlinks-int-)
* [Parser.getHyperlinks(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-int--PageAreaOptions-)

Voir les exemples d'utilisation là-bas.

## Constructors

| Constructor | Description |
| --- | --- |
|  | [PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)](#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initialise une nouvelle instance de la classe [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea). |
|
## Methods

| Method | Description |
| --- | --- |
|  | [getText()](#getText--) | Obtient le texte du lien hypertexte. |
|
|  | [getUrl()](#getUrl--) | Obtient l'URL du lien hypertexte. |
|
### PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle) {#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)
```


Initialise une nouvelle instance de la classe [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea).


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
|  | texte | java.lang.String | Le texte du lien hypertexte. |
|
|  | url | java.lang.String | L'URL du lien hypertexte. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | La page qui contient le lien hypertexte. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | La zone rectangulaire qui contient le lien hypertexte. |
|

### getText() {#getText--}
```
public String getText()
```


Obtient le texte du lien hypertexte.


**Returns:**
java.lang.String - Une valeur de chaîne qui représente le texte du lien hypertexte.

### getUrl() {#getUrl--}
```
public String getUrl()
```


Obtient l'URL du lien hypertexte.


**Returns:**
java.lang.String - Une valeur de chaîne qui représente l'URL du lien hypertexte.

