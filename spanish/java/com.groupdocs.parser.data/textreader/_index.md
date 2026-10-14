---
title: "TextReader"
second_title: "Referencia de la API de GroupDocs.Parser for Java"
description: "Representa un lector que puede leer una serie secuencial de caracteres."
type: docs
weight: 29
url: /es/java/com.groupdocs.parser.data/textreader/
---
**Inheritance:**
java.lang.Object, java.io.Reader
```
public abstract class TextReader extends Reader
```

Representa un lector que puede leer una serie secuencial de caracteres.

## Constructores

| Constructor | Descripción |
| --- | --- |
| [TextReader()](#TextReader--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [markSupported()](#markSupported--) |  |
|  | [readLine()](#readLine--) | Lee una línea de caracteres del lector de texto y devuelve los datos como una cadena. |
|
|  | [readToEnd()](#readToEnd--) | Lee todos los caracteres desde la posición actual hasta el final del lector de texto y los devuelve como una sola cadena. |
|
|  | [dispose()](#dispose--) | Libera todos los recursos utilizados por el objeto [TextReader](../../com.groupdocs.parser.data/textreader). |
|
### TextReader() {#TextReader--}
```
public TextReader()
```


### markSupported() {#markSupported--}
```
public boolean markSupported()
```




**Returns:**
boolean
### readLine() {#readLine--}
```
public abstract String readLine()
```


Lee una línea de caracteres del lector de texto y devuelve los datos como una cadena.


**Returns:**
java.lang.String - La siguiente línea del lector, o  null  si se han leído todos los caracteres.

### readToEnd() {#readToEnd--}
```
public abstract String readToEnd()
```


Lee todos los caracteres desde la posición actual hasta el final del lector de texto y los devuelve como una sola cadena.


**Returns:**
java.lang.String - Una cadena que contiene todos los caracteres desde la posición actual hasta el final del lector de texto.

### dispose() {#dispose--}
```
public void dispose()
```


Libera todos los recursos utilizados por el objeto [TextReader](../../com.groupdocs.parser.data/textreader).


