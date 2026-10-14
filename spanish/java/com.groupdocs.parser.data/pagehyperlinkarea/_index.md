---
title: "PageHyperlinkArea"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa un área de página que se utiliza para representar un hipervínculo en la página."
type: docs
weight: 20
url: /es/java/com.groupdocs.parser.data/pagehyperlinkarea/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.data.PageArea](../../com.groupdocs.parser.data/pagearea)
```
public class PageHyperlinkArea extends PageArea
```

Representa un área de página que se utiliza para representar un hipervínculo en la página.

Una instancia de la clase [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea) se usa como valor de retorno de los siguientes métodos:

* [Parser.getHyperlinks()](../../com.groupdocs.parser/parser#getHyperlinks--)
* [Parser.getHyperlinks(PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-PageAreaOptions-)
* [Parser.getHyperlinks(int)](../../com.groupdocs.parser/parser#getHyperlinks-int-)
* [Parser.getHyperlinks(int, PageAreaOptions)](../../com.groupdocs.parser/parser#getHyperlinks-int--PageAreaOptions-)

Vea los ejemplos de uso allí.

## Constructores

| Constructor | Descripción |
| --- | --- |
|  | [PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)](#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-) | Inicializa una nueva instancia de la clase [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea). |
|
## Métodos

| Método | Descripción |
| --- | --- |
|  | [getText()](#getText--) | Obtiene el texto del hipervínculo. |
|
|  | [getUrl()](#getUrl--) | Obtiene la URL del hipervínculo. |
|
### PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle) {#PageHyperlinkArea-java.lang.String-java.lang.String-com.groupdocs.parser.data.Page-com.groupdocs.parser.data.Rectangle-}
```
public PageHyperlinkArea(String text, String url, Page page, Rectangle rectangle)
```


Inicializa una nueva instancia de la clase [PageHyperlinkArea](../../com.groupdocs.parser.data/pagehyperlinkarea).


**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
|  | texto | java.lang.String | El texto del hipervínculo. |
|
|  | url | java.lang.String | La URL del hipervínculo. |
|
|  | page | [Page](../../com.groupdocs.parser.data/page) | La página que contiene el hipervínculo. |
|
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | El área rectangular que contiene el hipervínculo. |
|

### getText() {#getText--}
```
public String getText()
```


Obtiene el texto del hipervínculo.


**Returns:**
java.lang.String - Un valor de cadena que representa el texto del hipervínculo.

### getUrl() {#getUrl--}
```
public String getUrl()
```


Obtiene la URL del hipervínculo.


**Returns:**
java.lang.String - Un valor de cadena que representa la URL del hipervínculo.

