---
title: "IPreviewPageRender"
second_title: "Java용 GroupDocs.Parser API 참조"
description: "문서 페이지가 렌더링되기 전에 호출되는 메서드를 나타냅니다."
type: docs
weight: 41
url: /ko/java/com.groupdocs.parser.options/ipreviewpagerender/
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

