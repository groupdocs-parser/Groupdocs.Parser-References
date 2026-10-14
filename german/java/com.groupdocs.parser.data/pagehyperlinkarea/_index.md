---
title: "PageHyperlinkArea"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt einen Seitenbereich dar, der verwendet wird, um einen Hyperlink auf der Seite zu repräsentieren."
type: docs
weight: 20
url: /de/java/com.groupdocs.parser.data/pagehyperlinkarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageHyperlinkArea extends PageArea
```

Stellt einen Seitenbereich dar, der verwendet wird, um einen Hyperlink auf der Seite zu repräsentieren.

Eine Instanz der Klasse [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) wird als Rückgabewert der folgenden Methoden verwendet:

* [Parser.getHyperlinks()](../../com.groupdocs.parser/parser#getHyperlinks--)
* [Parser.getHyperlinks(PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-PageAreaOptions-)
* [Parser.getHyperlinks(int)](../../com.groupdocs.parser/parser#getHyperlinks-int-)
* [Parser.getHyperlinks(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-int--PageAreaOptions-)

Siehe dort die Anwendungsbeispiele.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)](#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initialisiert eine neue Instanz der Klasse [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getText()](#getText--) | Ruft den Hyperlink-Text ab. |
|
|  | [getUrl()](#getUrl--) | Ruft die Hyperlink-URL ab. |
|
### PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle) {#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)
```


Initialisiert eine neue Instanz der Klasse [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Text | java.lang.String | Der Hyperlink-Text. |
|
|  | url | java.lang.String | Die Hyperlink-URL. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Die Seite, die den Hyperlink enthält. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Der rechteckige Bereich, der den Hyperlink enthält. |
|

### getText() {#getText--}
```
public String getText()
```


Ruft den Hyperlink-Text ab.


**Returns:**
java.lang.String - Ein Zeichenkettenwert, der den Hyperlink-Text darstellt.

### getUrl() {#getUrl--}
```
public String getUrl()
```


Ruft die Hyperlink-URL ab.


**Returns:**
java.lang.String - Ein Zeichenkettenwert, der die Hyperlink-URL darstellt.

