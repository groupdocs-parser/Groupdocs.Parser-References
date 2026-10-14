---
title: "TextReader"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta un lettore che può leggere una serie sequenziale di caratteri."
type: docs
weight: 29
url: /it/java/com.groupdocs.parser.data/textreader/
---
**Inheritance:**
java.lang.Object, java.io.Reader
```
public abstract class TextReader extends Reader
```

Rappresenta un lettore che può leggere una serie sequenziale di caratteri.

## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [TextReader()](#TextReader--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [markSupported()](#markSupported--) |  |
|  | [readLine()](#readLine--) | Legge una riga di caratteri dal lettore di testo e restituisce i dati come stringa. |
|
|  | [readToEnd()](#readToEnd--) | Legge tutti i caratteri dalla posizione corrente fino alla fine del lettore di testo e li restituisce come una singola stringa. |
|
|  | [dispose()](#dispose--) | Rilascia tutte le risorse utilizzate dall'oggetto [TextReader](../../com.groupdocs.parser.data/textreader). |
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


Legge una riga di caratteri dal lettore di testo e restituisce i dati come stringa.


**Returns:**
java.lang.String - La riga successiva dal lettore, o  null  se tutti i caratteri sono stati letti.

### readToEnd() {#readToEnd--}
```
public abstract String readToEnd()
```


Legge tutti i caratteri dalla posizione corrente fino alla fine del lettore di testo e li restituisce come una singola stringa.


**Returns:**
java.lang.String - Una stringa che contiene tutti i caratteri dalla posizione corrente fino alla fine del lettore di testo.

### dispose() {#dispose--}
```
public void dispose()
```


Rilascia tutte le risorse utilizzate dall'oggetto [TextReader](../../com.groupdocs.parser.data/textreader).


