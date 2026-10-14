---
title: "TextStyle"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta lo stile del testo, come il nome del carattere, la dimensione del carattere e così via."
type: docs
weight: 30
url: /it/java/com.groupdocs.parser.data/textstyle/
---
**Inheritance:**
java.lang.Object
```
public final class TextStyle
```

Rappresenta lo stile del testo come un nome di carattere, una dimensione del carattere e così via.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)](#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-) | Inizializza una nuova istanza della classe [TextStyle](../../com.groupdocs.parser.data/textstyle). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getName()](#getName--) | Restituisce il nome dello stile. |
|
|  | [getFontName()](#getFontName--) | Restituisce il nome del carattere. |
|
|  | [getFontSize()](#getFontSize--) | Ottiene la dimensione del carattere. |
|
|  | [isBold()](#isBold--) | Ottiene il valore che indica se il carattere è in grassetto. |
|
|  | [isItalic()](#isItalic--) | Ottiene il valore che indica se il carattere è in corsivo. |
|
| [equals(Object o)](#equals-java.lang.Object-) |  |
| [hashCode()](#hashCode--) |  |
### TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic) {#TextStyle-java.lang.String-java.lang.String-double-boolean-boolean-}
```
public TextStyle(String name, String fontName, double fontSize, boolean bold, boolean italic)
```


Inizializza una nuova istanza della classe [TextStyle](../../com.groupdocs.parser.data/textstyle).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | name | java.lang.String | Il nome dello stile. |
|
|  | fontName | java.lang.String | Il nome del carattere. |
|
|  | fontSize | double | La dimensione del carattere. |
|
|  | bold | boolean | Il valore che indica se il carattere è in grassetto. |
|
|  | italic | boolean | Il valore che indica se il carattere è in corsivo. |
|

### getName() {#getName--}
```
public String getName()
```


Restituisce il nome dello stile.


**Returns:**
java.lang.String - Un valore stringa che rappresenta il nome dello stile.

### getFontName() {#getFontName--}
```
public String getFontName()
```


Restituisce il nome del carattere.


**Returns:**
java.lang.String - Un valore stringa che rappresenta il nome del carattere.

### getFontSize() {#getFontSize--}
```
public double getFontSize()
```


Ottiene la dimensione del carattere.


**Returns:**
double - Un valore double che rappresenta la dimensione del carattere.

### isBold() {#isBold--}
```
public boolean isBold()
```


Ottiene il valore che indica se il carattere è in grassetto.


**Returns:**
boolean -  true  se il carattere è in grassetto; altrimenti,  false .

### isItalic() {#isItalic--}
```
public boolean isItalic()
```


Ottiene il valore che indica se il carattere è in corsivo.


**Returns:**
boolean -  true  se il carattere è in corsivo; altrimenti,  false .

### equals(Object o) {#equals-java.lang.Object-}
```
public boolean equals(Object o)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object |  |

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int
