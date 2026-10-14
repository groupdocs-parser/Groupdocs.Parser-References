---
title: "TextReader"
second_title: "GroupDocs.Parser for Java API-Referenz"
description: "Stellt einen Reader dar, der eine sequenzielle Reihe von Zeichen lesen kann."
type: docs
weight: 29
url: /de/java/com.groupdocs.parser.data/textreader/
---
**Inheritance:**
java.lang.Object, java.io.Reader
```
public abstract class TextReader extends Reader
```

Stellt einen Reader dar, der eine sequenzielle Reihe von Zeichen lesen kann.

## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [TextReader()](#TextReader--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [markSupported()](#markSupported--) |  |
|  | [readLine()](#readLine--) | Liest eine Zeile von Zeichen aus dem TextReader und gibt die Daten als Zeichenkette zurück. |
|
|  | [readToEnd()](#readToEnd--) | Liest alle Zeichen von der aktuellen Position bis zum Ende des TextReaders und gibt sie als eine Zeichenkette zurück. |
|
|  | [dispose()](#dispose--) | Gibt alle von dem [TextReader](../../com.groupdocs.parser.data/textreader)-Objekt verwendeten Ressourcen frei. |
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


Liest eine Zeile von Zeichen aus dem TextReader und gibt die Daten als Zeichenkette zurück.


**Returns:**
java.lang.String - Die nächste Zeile aus dem Reader, oder  null  wenn alle Zeichen gelesen wurden.

### readToEnd() {#readToEnd--}
```
public abstract String readToEnd()
```


Liest alle Zeichen von der aktuellen Position bis zum Ende des TextReaders und gibt sie als eine Zeichenkette zurück.


**Returns:**
java.lang.String - Eine Zeichenkette, die alle Zeichen von der aktuellen Position bis zum Ende des TextReaders enthält.

### dispose() {#dispose--}
```
public void dispose()
```


Gibt alle von dem [TextReader](../../com.groupdocs.parser.data/textreader)-Objekt verwendeten Ressourcen frei.


