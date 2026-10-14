---
title: "IPreviewPageRender"
second_title: "GroupDocs.Parser for Java API संदर्भ"
description: "एक विधि को दर्शाता है जो दस्तावेज़ पृष्ठ को रेंडर करने से पहले कॉल की जाती है।"
type: docs
weight: 41
url: /hi/java/com.groupdocs.parser.options/ipreviewpagerender/
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

