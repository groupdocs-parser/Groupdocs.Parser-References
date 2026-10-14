---
title: "Rectangle"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta un'area rettangolare."
type: docs
weight: 26
url: /it/java/com.groupdocs.parser.data/rectangle/
---
**Inheritance:**
java.lang.Object
```
public class Rectangle
```

Rappresenta un'area rettangolare.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
|  | [Rectangle(double left, double top, double right, double bottom)](#Rectangle-double-double-double-double-) | Inizializza una nuova istanza della classe [Rectangle](../../com.groupdocs.parser.data/rectangle). |
|
|  | [Rectangle(Point position, Size size)](#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-) | Inizializza una nuova istanza della classe [Rectangle](../../com.groupdocs.parser.data/rectangle). |
|
## Metodi

| Metodo | Descrizione |
| --- | --- |
|  | [getLeft()](#getLeft--) | Restituisce la coordinata x del bordo sinistro dell'area rettangolare. |
|
|  | [getTop()](#getTop--) | Restituisce la coordinata y del bordo superiore dell'area rettangolare. |
|
|  | [getRight()](#getRight--) | Restituisce la coordinata x del bordo destro dell'area rettangolare. |
|
|  | [getBottom()](#getBottom--) | Restituisce la coordinata y del bordo inferiore dell'area rettangolare. |
|
|  | [getPosition()](#getPosition--) | Restituisce le coordinate dell'angolo superiore sinistro dell'area rettangolare. |
|
|  | [getSize()](#getSize--) | Restituisce le dimensioni. |
|
| [toString()](#toString--) |  |
### Rectangle(double left, double top, double right, double bottom) {#Rectangle-double-double-double-double-}
```
public Rectangle(double left, double top, double right, double bottom)
```


Inizializza una nuova istanza della classe [Rectangle](../../com.groupdocs.parser.data/rectangle).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | sinistra | double | La coordinata x del bordo sinistro dell'area rettangolare. |
|
|  | alto | double | La coordinata y del bordo superiore dell'area rettangolare. |
|
|  | destra | double | La coordinata x del bordo destro dell'area rettangolare. |
|
|  | in basso | double | La coordinata y del bordo inferiore dell'area rettangolare. |
|

### Rectangle(Point position, Size size) {#Rectangle-com.groupdocs.parser.data.Point-com.groupdocs.parser.data.Size-}
```
public Rectangle(Point position, Size size)
```


Inizializza una nuova istanza della classe [Rectangle](../../com.groupdocs.parser.data/rectangle).


**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
|  | position | [Point](../../com.groupdocs.parser.data/point) | Le coordinate dell'angolo superiore sinistro dell'area rettangolare. |
|
|  | size | [Size](../../com.groupdocs.parser.data/size) | Le dimensioni dell'area rettangolare. |
|

### getLeft() {#getLeft--}
```
public double getLeft()
```


Restituisce la coordinata x del bordo sinistro dell'area rettangolare.


**Returns:**
double - Un valore double che rappresenta la coordinata x del bordo sinistro dell'area rettangolare.

### getTop() {#getTop--}
```
public double getTop()
```


Restituisce la coordinata y del bordo superiore dell'area rettangolare.


**Returns:**
double - Un valore double che rappresenta la coordinata y del bordo superiore dell'area rettangolare.

### getRight() {#getRight--}
```
public double getRight()
```


Restituisce la coordinata x del bordo destro dell'area rettangolare.


**Returns:**
double - Un valore double che rappresenta la coordinata x del bordo destro dell'area rettangolare.

### getBottom() {#getBottom--}
```
public double getBottom()
```


Restituisce la coordinata y del bordo inferiore dell'area rettangolare.


**Returns:**
double - Un valore double che rappresenta la coordinata y del bordo inferiore dell'area rettangolare.

### getPosition() {#getPosition--}
```
public Point getPosition()
```


Restituisce le coordinate dell'angolo superiore sinistro dell'area rettangolare.


**Returns:**
[Point](../../com.groupdocs.parser.data/point) - An instance of [Point](../../com.groupdocs.parser.data/point) class that represents the coordinates of the upper-left corner of the rectangular area.

### getSize() {#getSize--}
```
public Size getSize()
```


Restituisce le dimensioni.


**Returns:**
[Size](../../com.groupdocs.parser.data/size) - An instance of [Size](../../com.groupdocs.parser.data/size) class that represents the size of the rectangular area.

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
