---
title: "TemplateField"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Tillhandahåller mallens textfält."
type: docs
weight: 12
url: /sv/java/com.groupdocs.parser.templates/templatefield/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateField extends TemplateItem
```

Tillhandahåller mallens textfält.

Textfält definieras av deras position på sidan. Det finns tre sätt att definiera ett textfält:

* Using the rectangular area: [TemplateFixedPosition](../../com.groupdocs.parser.templates/templatefixedposition)
* Using the regular expression: [TemplateRegexPosition](../../com.groupdocs.parser.templates/templateregexposition)
* Using the linked field: [TemplateLinkedPosition](../../com.groupdocs.parser.templates/templatelinkedposition)

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
|  | [TemplateField(TemplatePosition position, String name)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-) | Initierar en ny instans av klassen [TemplateField](../../com.groupdocs.parser.templates/templatefield). |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-) | Initierar en ny instans av klassen [TemplateField](../../com.groupdocs.parser.templates/templatefield) med namn i STORA BOKSTÄVER. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-) | Initierar en ny instans av klassen [TemplateField](../../com.groupdocs.parser.templates/templatefield) med namn i STORA BOKSTÄVER. |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-) | Initierar en ny instans av klassen [TemplateField](../../com.groupdocs.parser.templates/templatefield). |
|
|  | [TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Initierar en ny instans av klassen [TemplateField](../../com.groupdocs.parser.templates/templatefield). |
|
## Metoder

| Metod | Beskrivning |
| --- | --- |
|  | [getPosition()](#getPosition--) | Hämtar värdet som beskriver hur man hittar mallfältet på dokumentsidan. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateField(TemplatePosition position, String name) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-}
```
public TemplateField(TemplatePosition position, String name)
```


Initierar en ny instans av klassen [TemplateField](../../com.groupdocs.parser.templates/templatefield).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Fältpositionen. |
|
|  | namn | java.lang.String | Fältnamnet. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex)
```


Initierar en ny instans av klassen [TemplateField](../../com.groupdocs.parser.templates/templatefield) med namn i STORA BOKSTÄVER.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Fältpositionen. |
|
|  | namn | java.lang.String | Fältnamnet. |
|
|  | pageIndex | java.lang.Integer | Ett heltalsvärde som representerar sidans index där mallobjektet är placerat;  null  om mallobjektet är placerat på någon sida. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth)
```


Initierar en ny instans av klassen [TemplateField](../../com.groupdocs.parser.templates/templatefield) med namn i STORA BOKSTÄVER.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Fältpositionen. |
|
|  | namn | java.lang.String | Fältnamnet. |
|
|  | pageIndex | java.lang.Integer | Ett heltalsvärde som representerar sidans index där mallobjektet är placerat;  null  om mallobjektet är placerat på någon sida. |
|
|  | pageWidth | java.lang.Double | Sidans bredd som användes för att skapa mallobjektet. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, boolean useUpperCaseName)
```


Initierar en ny instans av klassen [TemplateField](../../com.groupdocs.parser.templates/templatefield).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Fältpositionen. |
|
|  | namn | java.lang.String | Fältnamnet. |
|
|  | pageIndex | java.lang.Integer | Ett heltalsvärde som representerar sidans index där mallobjektet är placerat;  null  om mallobjektet är placerat på någon sida. |
|
|  | useUpperCaseName | boolean | Värdet som indikerar om ett  name  konverteras till STORA BOKSTÄVER. |
|

### TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateField-com.groupdocs.parser.templates.TemplatePosition-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateField(TemplatePosition position, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Initierar en ny instans av klassen [TemplateField](../../com.groupdocs.parser.templates/templatefield).


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
|  | position | [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) | Fältpositionen. |
|
|  | namn | java.lang.String | Fältnamnet. |
|
|  | pageIndex | java.lang.Integer | Ett heltalsvärde som representerar sidans index där mallobjektet är placerat;  null  om mallobjektet är placerat på någon sida. |
|
|  | pageWidth | java.lang.Double | Sidans bredd som användes för att skapa mallobjektet. |
|
|  | useUpperCaseName | boolean | Värdet som indikerar om ett  name  konverteras till STORA BOKSTÄVER. |
|

### getPosition() {#getPosition--}
```
public TemplatePosition getPosition()
```


Hämtar värdet som beskriver hur man hittar mallfältet på dokumentsidan.


**Returns:**
[TemplatePosition](../../com.groupdocs.parser.templates/templateposition) - An instance of [TemplatePosition](../../com.groupdocs.parser.templates/templateposition) descendant class.

### scale(double factor) {#scale-double-}
```
public TemplateItem scale(double factor)
```


Skapar en kopia av det aktuella objektet med alla koordinater skalade med den angivna faktorn.


**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| faktor | double |  |

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem)
