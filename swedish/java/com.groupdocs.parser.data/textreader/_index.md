---
title: "TextReader"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar en läsare som kan läsa en sekventiell serie av tecken."
type: docs
weight: 29
url: /sv/java/com.groupdocs.parser.data/textreader/
---
**Inheritance:**
java.lang.Object, java.io.Reader
```
public abstract class TextReader extends Reader
```

Representerar en läsare som kan läsa en sekventiell serie av tecken.

## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [TextReader()](#TextReader--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [markSupported()](#markSupported--) |  |
|  | [readLine()](#readLine--) | Läser en rad tecken från textläsaren och returnerar data som en sträng. |
|
|  | [readToEnd()](#readToEnd--) | Läser alla tecken från den aktuella positionen till slutet av textläsaren och returnerar dem som en sträng. |
|
|  | [dispose()](#dispose--) | Frigör alla resurser som används av objektet [TextReader](../../com.groupdocs.parser.data/textreader). |
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


Läser en rad tecken från textläsaren och returnerar data som en sträng.


**Returns:**
java.lang.String - Nästa rad från läsaren, eller  null  om alla tecken har lästs.

### readToEnd() {#readToEnd--}
```
public abstract String readToEnd()
```


Läser alla tecken från den aktuella positionen till slutet av textläsaren och returnerar dem som en sträng.


**Returns:**
java.lang.String - En sträng som innehåller alla tecken från den aktuella positionen till slutet av textläsaren.

### dispose() {#dispose--}
```
public void dispose()
```


Frigör alla resurser som används av objektet [TextReader](../../com.groupdocs.parser.data/textreader).


