---
title: IReleasePageStream
second_title: GroupDocs.Parser for Java API Reference
description: Represents a method which releases the stream created by the  delegate.
type: docs
weight: 41
url: /java/com.groupdocs.parser.options/ireleasepagestream/
---```
public interface IReleasePageStream
```

Represents a method which releases the stream created by the [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) delegate.
## Methods

| Method | Description |
| --- | --- |
| [releasePageStream(int pageNumber, OutputStream pageStream)](#releasePageStream-int-java.io.OutputStream-) | Releases the stream created by the [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) delegate. |
### releasePageStream(int pageNumber, OutputStream pageStream) {#releasePageStream-int-java.io.OutputStream-}
```
public abstract void releasePageStream(int pageNumber, OutputStream pageStream)
```


Releases the stream created by the [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) delegate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageNumber | int | The page number of a generated page preview. |
| pageStream | java.io.OutputStream | The stream containing the generated page preview. |

