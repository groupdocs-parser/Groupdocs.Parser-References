---
title: "Size"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta una dimensione."
type: docs
weight: 28
url: /it/java/com.groupdocs.parser.data/size/
---
**Inheritance:**
java.lang.Object
```
public class Size
```

Rappresenta una dimensione.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [Size(double width, double height)](#Size-double-double-) | Inizializza una nuova istanza della classe [Size](../../com.groupdocs.parser.data/size). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getWidth()](#getWidth--) | Restituisce la larghezza. |
|
|  | [getHeight()](#getHeight--) | Restituisce l'altezza. |
|
|  | [isEmpty()](#isEmpty--) | Restituisce un valore che indica se la dimensione è vuota. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Converte la rappresentazione stringa di una dimensione nella sua equivalenza di classe. |
|
| [toString()](#toString--) |  |
### Size(double width, double height) {#Size-double-double-}
```
public Size(double width, double height)
```


Inizializza una nuova istanza della classe [Size](../../com.groupdocs.parser.data/size).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | width | double | La larghezza in pixel. |
|
|  | height | double | L'altezza in pixel. |
|

### getWidth() {#getWidth--}
```
public double getWidth()
```


Restituisce la larghezza.


**Returns:**
double - Un valore double che rappresenta la larghezza in pixel.

### getHeight() {#getHeight--}
```
public double getHeight()
```


Restituisce l'altezza.


**Returns:**
double - Un valore double che rappresenta l'altezza in pixel.

### isEmpty() {#isEmpty--}
```
public boolean isEmpty()
```


Restituisce un valore che indica se la dimensione è vuota.


**Returns:**
boolean -  true  se la  larghezza  e  l'altezza  sono zero; altrimenti,  false .

### parse(String s) {#parse-java.lang.String-}
```
public static Size parse(String s)
```


Converte la rappresentazione stringa di una dimensione nella sua equivalente di classe. Un valore di ritorno indica se la conversione è riuscita o fallita.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | s | java.lang.String | Una stringa contenente una dimensione da convertire. |
|

**Returns:**
[Size](../../com.groupdocs.parser.data/size) - The instance of [Size](../../com.groupdocs.parser.data/size) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
