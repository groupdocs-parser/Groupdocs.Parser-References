---
title: "Point"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta un punto."
type: docs
weight: 25
url: /it/java/com.groupdocs.parser.data/point/
---
**Inheritance:**
java.lang.Object
```
public class Point
```

Rappresenta un punto.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [Point(double x, double y)](#Point-double-double-) | Inizializza una nuova istanza della classe [Point](../../com.groupdocs.parser.data/point). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getX()](#getX--) | Ottiene la coordinata x. |
|
|  | [getY()](#getY--) | Ottiene la coordinata y. |
|
|  | [parse(String s)](#parse-java.lang.String-) | Converte la rappresentazione testuale di un punto nella sua equivalenza di classe. |
|
| [toString()](#toString--) |  |
### Point(double x, double y) {#Point-double-double-}
```
public Point(double x, double y)
```


Inizializza una nuova istanza della classe [Point](../../com.groupdocs.parser.data/point).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | x | double | La coordinata x. |
|
|  | y | double | La coordinata y. |
|

### getX() {#getX--}
```
public double getX()
```


Ottiene la coordinata x.


**Returns:**
double - Un valore double che rappresenta la coordinata x.

### getY() {#getY--}
```
public double getY()
```


Ottiene la coordinata y.


**Returns:**
double - Un valore double che rappresenta la coordinata y.

### parse(String s) {#parse-java.lang.String-}
```
public static Point parse(String s)
```


Converte la rappresentazione stringa di un punto nella sua equivalenza di classe. Un valore di ritorno indica se la conversione è riuscita o è fallita.


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | s | java.lang.String | Una stringa contenente un punto da convertire. |
|

**Returns:**
[Point](../../com.groupdocs.parser.data/point) - The instance of [Point](../../com.groupdocs.parser.data/point) class that is equivalent to the value specified in  s  parameter.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
