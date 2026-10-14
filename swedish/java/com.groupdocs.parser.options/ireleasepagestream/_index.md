---
title: "IReleasePageStream"
second_title: "GroupDocs.Parser för Java API-referens"
description: "Representerar en metod som frigör strömmen som skapats av delegaten."
type: docs
weight: 42
url: /sv/java/com.groupdocs.parser.options/ireleasepagestream/
---```
public interface IReleasePageStream
```

Represents a method which releases the stream created by the [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) delegate.

## Methods

| Method | Description |
| --- | --- |
| [releasePageStream(int pageNumber, OutputStream pageStream)](#releasePageStream-int-java.io.OutputStream-) | Releases the stream created by the [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) delegate.
 |
### releasePageStream(int pageNumber, OutputStream pageStream) {#releasePageStream-int-java.io.OutputStream-}
```
public abstract void releasePageStream(int pageNumber, OutputStream pageStream)
```


Releases the stream created by the [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) delegate.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageNumber | int | The page number of a generated page preview.
 |
| pageStream | java.io.OutputStream | The stream containing the generated page preview.
 |

