---
title: "PageHyperlinkArea"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar ett sidområde som används för att representera en hyperlänk på sidan."
type: docs
weight: 20
url: /sv/java/com.groupdocs.parser.data/pagehyperlinkarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageHyperlinkArea extends PageArea
```

Representerar ett sidområde som används för att representera en hyperlänk på sidan.

En instans av klassen [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) används som returvärde för följande metoder:

* [Parser.getHyperlinks()](../../com.groupdocs.parser/parser#getHyperlinks--)
* [Parser.getHyperlinks(PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-PageAreaOptions-)
* [Parser.getHyperlinks(int)](../../com.groupdocs.parser/parser#getHyperlinks-int-)
* [Parser.getHyperlinks(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-int--PageAreaOptions-)

Se användningsexemplen där.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)](#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initierar en ny instans av klassen [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getText()](#getText--) | Hämtar hyperlänktexten. |
|
|  | [getUrl()](#getUrl--) | Hämtar hyperlänkens URL. |
|
### PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle) {#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)
```


Initierar en ny instans av klassen [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | text | java.lang.String | Hyperlänktexten. |
|
|  | url | java.lang.String | Hyperlänkens URL. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Sidan som innehåller hyperlänken. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Det rektangulära området som innehåller hyperlänken. |
|

### getText() {#getText--}
```
public String getText()
```


Hämtar hyperlänktexten.


**Returns:**
java.lang.String - Ett strängvärde som representerar hyperlänktext.

### getUrl() {#getUrl--}
```
public String getUrl()
```


Hämtar hyperlänkens URL.


**Returns:**
java.lang.String - Ett strängvärde som representerar hyperlänkens URL.

