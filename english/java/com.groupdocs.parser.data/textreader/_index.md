---
title: TextReader
second_title: GroupDocs.Parser for Java API Reference
description: Represents a reader that can read a sequential series of characters.
type: docs
weight: 29
url: /java/com.groupdocs.parser.data/textreader/
---
**Inheritance:**
java.lang.Object, java.io.Reader
```
public abstract class TextReader extends Reader
```

Represents a reader that can read a sequential series of characters.
## Constructors

| Constructor | Description |
| --- | --- |
| [TextReader()](#TextReader--) |  |
## Methods

| Method | Description |
| --- | --- |
| [markSupported()](#markSupported--) |  |
| [readLine()](#readLine--) | Reads a line of characters from the text reader and returns the data as a string. |
| [readToEnd()](#readToEnd--) | Reads all characters from the current position to the end of the text reader and returns them as one string. |
| [dispose()](#dispose--) | Releases all resources used by [TextReader](../../com.groupdocs.parser.data/textreader) object. |
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


Reads a line of characters from the text reader and returns the data as a string.

**Returns:**
java.lang.String - The next line from the reader, or  null  if all characters have been read.
### readToEnd() {#readToEnd--}
```
public abstract String readToEnd()
```


Reads all characters from the current position to the end of the text reader and returns them as one string.

**Returns:**
java.lang.String - A string that contains all characters from the current position to the end of the text reader.
### dispose() {#dispose--}
```
public void dispose()
```


Releases all resources used by [TextReader](../../com.groupdocs.parser.data/textreader) object.

