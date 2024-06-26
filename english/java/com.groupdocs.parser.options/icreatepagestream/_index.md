---
title: ICreatePageStream
second_title: GroupDocs.Parser for Java API Reference
description: Represents a delegate that returns a stream to write page preview data.
type: docs
weight: 38
url: /java/com.groupdocs.parser.options/icreatepagestream/
---```
public interface ICreatePageStream
```

Represents a delegate that returns a stream to write page preview data.
## Methods

| Method | Description |
| --- | --- |
| [createPageStream(int pageNumber)](#createPageStream-int-) | Returns a stream to write page preview data. |
### createPageStream(int pageNumber) {#createPageStream-int-}
```
public abstract OutputStream createPageStream(int pageNumber)
```


Returns a stream to write page preview data.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageNumber | int | The page number of a page to generate a thumbnail. |

**Returns:**
java.io.OutputStream - The stream to write the page preview.
