---
title: "PageTextArea"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt einen Seiten‑Text‑Bereich dar, der verwendet wird, um einen Textwert im Vorlagen‑Parsing oder Formular‑Parsing zu repräsentieren."
type: docs
weight: 24
url: /de/java/com.groupdocs.parser.data/pagetextarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageTextArea extends PageArea
```

Stellt einen Seiten‑Text‑Bereich dar, der verwendet wird, um einen Textwert im Vorlagen‑Parsing oder Formular‑Parsing zu repräsentieren.

Eine Instanz der Klasse [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) wird als Rückgabewert der folgenden Methoden verwendet:

* [Parser.getTextAreas()](../../com.groupdocs.parser/parser#getTextAreas--)
* [Parser.getTextAreas(PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-PageTextAreaOptions-)
* [Parser.getTextAreas(int)](../../com.groupdocs.parser/parser#getTextAreas-int-)
* [Parser.getTextAreas(int, PageTextAreaOptions)](../../com.groupdocs.parser/parser#getTextAreas-int--PageTextAreaOptions-)

Auch eine Instanz der Klasse [PageTextArea](../../com.groupdocs.parser.data/pagetextarea) wird als Wert der Eigenschaft [PageArea](../../com.groupdocs.parser.data/pagearea) verwendet.
\*

Siehe dort die Anwendungsbeispiele.

Der Textbereich kann einfach oder zusammengesetzt sein. Im ersten Fall enthält er einen Text, der durch einen rechteckigen Bereich begrenzt ist.
Im zweiten Fall enthält er andere Textbereiche; Text- und Tabelleneigenschaften werden von untergeordneten Textbereichen berechnet.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
|  | [PageTextArea(String text, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initialisiert eine neue Instanz der Klasse [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
|  | [PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)](#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Initialisiert eine neue Instanz der Klasse [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
|  | [PageTextArea(Iterable<PageTextArea> areas, Page page)](#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-) | Initialisiert eine neue Instanz der Klasse [PageTextArea](../../com.groupdocs.parser.data/pagetextarea). |
|
## Methoden

| Methode | Beschreibung |
| --- | --- |
|  | [getText()](#getText--) | Liefert den Text. |
|
|  | [getBaseLine()](#getBaseLine--) | Ruft die Grundlinie ab. |
|
|  | [getTextStyle()](#getTextStyle--) | Ruft den Textstil wie Schriftgröße, Schriftname und so weiter ab. |
|
|  | [getAreas()](#getAreas--) | Ruft die Sammlung von untergeordneten Textseitenbereichen ab. |
|
### PageTextArea(String text, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Page page, Rectangle rectangle)
```


Initialisiert eine neue Instanz der Klasse [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Text | java.lang.String | Der Wert des Textes. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Die Seite, die den Textbereich enthält. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Der rechteckige Bereich, der den Textbereich enthält. |
|

### PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle) {#PageTextArea-java.lang.String-java.lang.Double-com.groupdocs.parser.data.TextStyle-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageTextArea(String text, Double baseLine, TextStyle textStyle, Page page, Rectangle rectangle)
```


Initialisiert eine neue Instanz der Klasse [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Text | java.lang.String | Der Wert des Textes. |
|
|  | baseLine | java.lang.Double | Die Grundlinie des Textes. |
|
|  | textStyle | [TextStyle](../../com.groupdocs.parser.data/textstyle) | Der Stil des Textes. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Die Seite, die den Textbereich enthält. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | Der rechteckige Bereich, der den Textbereich enthält. |
|

### PageTextArea(Iterable<PageTextArea> areas, Page page) {#PageTextArea-java.lang.Iterable-com.groupdocs.parser.data.PageTextArea--com.groupdocs.parser.data.Page-}
```
public PageTextArea(Iterable<PageTextArea> areas, Page page)
```


Initialisiert eine neue Instanz der Klasse [PageTextArea](../../com.groupdocs.parser.data/pagetextarea).


**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
|  | Bereiche | java.lang.Iterable<com.groupdocs.parser.data.PageTextArea> | Die Sammlung von untergeordneten Textseitenbereichen. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | Die Seite, die den Textbereich enthält. |
|

### getText() {#getText--}
```
public String getText()
```


Liefert den Text.


**Returns:**
java.lang.String - Ein Zeichenkettenwert, der einen Wert des Textseitenbereichs darstellt.

### getBaseLine() {#getBaseLine--}
```
public double getBaseLine()
```


Ruft die Grundlinie ab.


**Returns:**
double - Ein double-Wert, der die Grundlinie darstellt.

### getTextStyle() {#getTextStyle--}
```
public TextStyle getTextStyle()
```


Ruft den Textstil wie Schriftgröße, Schriftname und so weiter ab.


**Returns:**
[TextStyle](../../com.groupdocs.parser.data/textstyle) - An instance of [TextStyle](../../com.groupdocs.parser.data/textstyle) class that represents the text style.

### getAreas() {#getAreas--}
```
public List<PageTextArea> getAreas()
```


Ruft die Sammlung von untergeordneten Textseitenbereichen ab.


**Returns:**
java.util.List<com.groupdocs.parser.data.PageTextArea> - Eine Sammlung von untergeordneten Textseitenbereichen; leer, wenn der Textseitenbereich keine Kinder hat.

