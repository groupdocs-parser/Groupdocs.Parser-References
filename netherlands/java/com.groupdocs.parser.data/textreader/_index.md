---
title: "TextReader"
second_title: "GroupDocs.Parser voor Java API-referentie"
description: "Stelt een lezer voor die een opeenvolgende reeks tekens kan lezen."
type: docs
weight: 29
url: /nl/java/com.groupdocs.parser.data/textreader/
---
**Inheritance:**
java.lang.Object, java.io.Reader
```
public abstract class TextReader extends Reader
```

Stelt een lezer voor die een opeenvolgende reeks tekens kan lezen.

## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [TextReader()](#TextReader--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [markSupported()](#markSupported--) |  |
|  | [readLine()](#readLine--) | Leest een regel tekens van de tekstlezer en retourneert de gegevens als een tekenreeks. |
|
|  | [readToEnd()](#readToEnd--) | Leest alle tekens vanaf de huidige positie tot het einde van de tekstlezer en retourneert ze als één tekenreeks. |
|
|  | [dispose()](#dispose--) | Geeft alle bronnen vrij die door het [TextReader](../../com.groupdocs.parser.data/textreader) object worden gebruikt. |
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


Leest een regel tekens van de tekstlezer en retourneert de gegevens als een tekenreeks.


**Returns:**
java.lang.String - De volgende regel van de lezer, of  null  als alle tekens zijn gelezen.

### readToEnd() {#readToEnd--}
```
public abstract String readToEnd()
```


Leest alle tekens vanaf de huidige positie tot het einde van de tekstlezer en retourneert ze als één tekenreeks.


**Returns:**
java.lang.String - Een tekenreeks die alle tekens bevat vanaf de huidige positie tot het einde van de tekstlezer.

### dispose() {#dispose--}
```
public void dispose()
```


Geeft alle bronnen vrij die door het [TextReader](../../com.groupdocs.parser.data/textreader) object worden gebruikt.


