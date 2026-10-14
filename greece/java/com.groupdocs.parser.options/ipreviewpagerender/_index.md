---
title: "IPreviewPageRender"
second_title: "GroupDocs.Parser για Java API Reference"
description: "Αναπαριστά μια μέθοδο που καλείται πριν αποδοθεί μια σελίδα εγγράφου."
type: docs
weight: 41
url: /el/java/com.groupdocs.parser.options/ipreviewpagerender/
---```
public interface IPreviewPageRender
```

Represents a method which is called before a document page is rendered.

## Methods

| Method | Description |
| --- | --- |
| [previewPageRender(PageRenderInfo info)](#previewPageRender-com.groupdocs.parser.options.PageRenderInfo-) | Provides the information of how a document page is rendered.
 |
### previewPageRender(PageRenderInfo info) {#previewPageRender-com.groupdocs.parser.options.PageRenderInfo-}
```
public abstract void previewPageRender(PageRenderInfo info)
```


Provides the information of how a document page is rendered.


**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| info | [PageRenderInfo](../../com.groupdocs.parser.options/pagerenderinfo) | The information of how a page is rendered.
 |

