---
title: "PageHyperlinkArea"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Stelt een paginagebied voor dat wordt gebruikt om een hyperlink op de pagina te representeren."
type: docs
weight: 20
url: /nl/java/com.groupdocs.parser.data/pagehyperlinkarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageHyperlinkArea extends PageArea
```

Stelt een paginagebied voor dat wordt gebruikt om een hyperlink op de pagina te representeren.

Een instantie van de klasse [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) wordt gebruikt als retourwaarde van de volgende methoden:

* [Parser.getHyperlinks()](../../com.groupdocs.parser/parser#getHyperlinks--)
* [Parser.getHyperlinks(PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-PageAreaOptions-)
* [Parser.getHyperlinks(int)](../../com.groupdocs.parser/parser#getHyperlinks-int-)
* [Parser.getHyperlinks(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-int--PageAreaOptions-)

Zie daar de gebruiksvoorbeelden.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
|  | [PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)](#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initialiseert een nieuwe instantie van de klasse [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea). |
|
## Methoden

| Methode | Beschrijving |
| --- | --- |
|  | [getText()](#getText--) | Haalt de hyperlinktekst op. |
|
|  | [getUrl()](#getUrl--) | Haalt de hyperlink-URL op. |
|
### PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle) {#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)
```


Initialiseert een nieuwe instantie van de klasse [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea).


**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
|  | tekst | java.lang.String | De hyperlinktekst. |
|
|  | url | java.lang.String | De hyperlink-URL. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | De pagina die de hyperlink bevat. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Het rechthoekige gebied dat de hyperlink bevat. |
|

### getText() {#getText--}
```
public String getText()
```


Haalt de hyperlinktekst op.


**Returns:**
java.lang.String - Een tekenreekswaarde die de hyperlinktekst weergeeft.

### getUrl() {#getUrl--}
```
public String getUrl()
```


Haalt de hyperlink-URL op.


**Returns:**
java.lang.String - Een tekenreekswaarde die de hyperlink-URL weergeeft.

