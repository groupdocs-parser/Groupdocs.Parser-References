---
title: "IPreviewPageRender"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "表示在渲染文档页面之前调用的方法。"
type: docs
weight: 41
url: /zh/java/com.groupdocs.parser.options/ipreviewpagerender/
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

