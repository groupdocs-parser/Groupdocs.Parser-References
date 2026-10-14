---
title: "ICreatePageStream"
second_title: "Riferimento API di GroupDocs.Parser per Java"
description: "Rappresenta un delegato che restituisce uno stream per scrivere i dati dell'anteprima della pagina."
type: docs
weight: 38
url: /it/java/com.groupdocs.parser.options/icreatepagestream/
---```
public interface ICreatePageStream
```

Represents a delegate that returns a stream to write page preview data.

## Methods

| Method | Description |
| --- | --- |
| [createPageStream(int pageNumber)](#createPageStream-int-) | Returns a stream to write page preview data.
 |
### createPageStream(int pageNumber) {#createPageStream-int-}
```
public abstract OutputStream createPageStream(int pageNumber)
```


Returns a stream to write page preview data.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageNumber | int | The page number of a page to generate a thumbnail.
 |

**Returns:**
java.io.OutputStream - The stream to write the page preview.

