---
title: "TemplateBarcode"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Fornisce il campo barcode del modello."
type: docs
weight: 11
url: /it/java/com.groupdocs.parser.templates/templatebarcode/
---
**Inheritance:**
java.lang.Object, [com.groupdocs.parser.templates.TemplateItem](../../com.groupdocs.parser.templates/templateitem)
```
public class TemplateBarcode extends TemplateItem
```

Fornisce il campo barcode del modello.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [TemplateBarcode(Rectangle rectangle, String name)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-) | Inizializza una nuova istanza della classe [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode). |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-) | Inizializza una nuova istanza della classe [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) con il nome MAIUSCOLO. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-) | Inizializza una nuova istanza della classe [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) con il nome MAIUSCOLO. |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-) | Inizializza una nuova istanza della classe [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode). |
|
|  | [TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)](#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-) | Inizializza una nuova istanza della classe [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getRectangle()](#getRectangle--) | Restituisce l'area rettangolare che contiene il campo barcode del modello. |
|
| [scale(double factor)](#scale-double-) |  |
### TemplateBarcode(Rectangle rectangle, String name) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-}
```
public TemplateBarcode(Rectangle rectangle, String name)
```


Inizializza una nuova istanza della classe [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare che contiene il campo barcode del modello. |
|
|  | name | java.lang.String | Il nome del campo barcode. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex)
```


Inizializza una nuova istanza della classe [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) con il nome MAIUSCOLO.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare che contiene il campo barcode del modello. |
|
|  | name | java.lang.String | Il nome del campo barcode. |
|
|  | pageIndex | java.lang.Integer | Un valore intero che rappresenta l'indice della pagina in cui si trova l'elemento del modello;  null  se l'elemento del modello si trova su qualsiasi pagina. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth)
```


Inizializza una nuova istanza della classe [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode) con il nome MAIUSCOLO.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare che contiene il campo barcode del modello. |
|
|  | name | java.lang.String | Il nome del campo barcode. |
|
|  | pageIndex | java.lang.Integer | Un valore intero che rappresenta l'indice della pagina in cui si trova l'elemento del modello;  null  se l'elemento del modello si trova su qualsiasi pagina. |
|
|  | pageWidth | java.lang.Double | La larghezza della pagina utilizzata per creare l'elemento modello. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, boolean useUpperCaseName)
```


Inizializza una nuova istanza della classe [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare che contiene il campo barcode del modello. |
|
|  | name | java.lang.String | Il nome del campo barcode. |
|
|  | pageIndex | java.lang.Integer | Un valore intero che rappresenta l'indice della pagina in cui si trova l'elemento del modello;  null  se l'elemento del modello si trova su qualsiasi pagina. |
|
|  | useUpperCaseName | boolean | Il valore che indica se un  nome  viene convertito in MAIUSCOLO. |
|

### TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName) {#TemplateBarcode-com.groupdocs.parser.data.Rectangle-java.lang.String-java.lang.Integer-java.lang.Double-boolean-}
```
public TemplateBarcode(Rectangle rectangle, String name, Integer pageIndex, Double pageWidth, boolean useUpperCaseName)
```


Inizializza una nuova istanza della classe [TemplateBarcode](../../com.groupdocs.parser.templates/templatebarcode).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | rectangle | [Rectangle](../../com.groupdocs.parser.data/rectangle) | L'area rettangolare che contiene il campo barcode del modello. |
|
|  | name | java.lang.String | Il nome del campo barcode. |
|
|  | pageIndex | java.lang.Integer | Un valore intero che rappresenta l'indice della pagina in cui si trova l'elemento del modello;  null  se l'elemento del modello si trova su qualsiasi pagina. |
|
|  | pageWidth | java.lang.Double | La larghezza della pagina utilizzata per creare l'elemento modello. |
|
|  | useUpperCaseName | boolean | Il valore che indica se un  nome  viene convertito in MAIUSCOLO. |
|

### getRectangle() {#getRectangle--}
```
public Rectangle getRectangle()
```


Restituisce l'area rettangolare che contiene il campo barcode del modello.


**Returns:**
[Rectangle](../../com.groupdocs.parser.data/rectangle) - An instance of [Rectangle](../../com.groupdocs.parser.data/rectangle) class that represents the rectangular area that contains the template barcode field.

### scale(double factor) {#scale-double-}
```
public TemplateItem scale(double factor)
```


Crea una copia dell'elemento corrente con tutte le coordinate scalate del fattore specificato.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fattore | double |  |

**Returns:**
[TemplateItem](../../com.groupdocs.parser.templates/templateitem)
