---
title: "TextReader"
second_title: "GroupDocs.Parser for Java API Reference"
description: "Представляет читатель, который может последовательно считывать символы."
type: docs
weight: 29
url: /ru/java/com.groupdocs.parser.data/textreader/
---
**Inheritance:**
java.lang.Object, java.io.Reader
```
public abstract class TextReader extends Reader
```

Представляет читатель, который может последовательно считывать символы.

## Конструкторы

| Конструктор | Описание |
| --- | --- |
| [TextReader()](#TextReader--) |  |
## Методы

| Метод | Описание |
| --- | --- |
| [markSupported()](#markSupported--) |  |
|  | [readLine()](#readLine--) | Считывает строку символов из текстового читателя и возвращает данные в виде строки. |
|
|  | [readToEnd()](#readToEnd--) | Считывает все символы от текущей позиции до конца текстового читателя и возвращает их в виде одной строки. |
|
|  | [dispose()](#dispose--) | Освобождает все ресурсы, используемые объектом [TextReader](../../com.groupdocs.parser.data/textreader). |
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


Считывает строку символов из текстового читателя и возвращает данные в виде строки.


**Returns:**
java.lang.String — следующая строка из читателя, или  null  если все символы уже считаны.

### readToEnd() {#readToEnd--}
```
public abstract String readToEnd()
```


Считывает все символы от текущей позиции до конца текстового читателя и возвращает их в виде одной строки.


**Returns:**
java.lang.String — строка, содержащая все символы от текущей позиции до конца текстового читателя.

### dispose() {#dispose--}
```
public void dispose()
```


Освобождает все ресурсы, используемые объектом [TextReader](../../com.groupdocs.parser.data/textreader).


