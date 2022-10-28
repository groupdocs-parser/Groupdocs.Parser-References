---
title: PreviewOptions
second_title: GroupDocs.Parser for Java API Reference
description: Provides options to sets requirements and stream delegates for preview generation.
type: docs
weight: 28
url: /java/com.groupdocs.parser.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

Provides options to sets requirements and stream delegates for preview generation.
## Constructors

| Constructor | Description |
| --- | --- |
| [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-) | Initializes a new instance of the [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) class causing the output stream to be closed. |
| [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-) | Initializes a new instance of [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) class causing the output stream to be returned to the client for further use. |
## Methods

| Method | Description |
| --- | --- |
| [getWidth()](#getWidth--) | Gets the page preview width. |
| [setWidth(int width)](#setWidth-int-) | Sets the page preview width. |
| [getHeight()](#getHeight--) | Gets the page preview height. |
| [setHeight(int height)](#setHeight-int-) | Sets the page preview height. |
| [getDpi()](#getDpi--) | Gets a dpi. |
| [setDpi(int dpi)](#setDpi-int-) | Sets a dpi. |
| [getPageNumbers()](#getPageNumbers--) | Gets an array of page numbers to generate previews. |
| [setPageNumbers(int[] pageNumbers)](#setPageNumbers-int---) | Sets an array of page numbers to generate previews. |
| [getPreviewFormat()](#getPreviewFormat--) | Gets the preview image format. |
| [setPreviewFormat(PreviewFormats previewFormat)](#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-) | Sets the preview image format. |
| [getCreatePageStream()](#getCreatePageStream--) | Gets an instance of the page stream creation delegate. |
| [setCreatePageStream(ICreatePageStream createPageStream)](#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-) | Sets an instance of the page stream creation delegate. |
| [getReleasePageStream()](#getReleasePageStream--) | Gets an instance of the page preview completion delegate. |
| [setReleasePageStream(IReleasePageStream releasePageStream)](#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-) | Sets an instance of the page preview completion delegate. |
| [getPreviewPageRender()](#getPreviewPageRender--) | Gets an instance of the page preview render info delegate. |
| [setPreviewPageRender(IPreviewPageRender previewPageRender)](#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-) | Sets an instance of the page preview render info delegate. |
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


Initializes a new instance of the [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) class causing the output stream to be closed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Creates a stream for a specific page preview. |

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


Initializes a new instance of [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) class causing the output stream to be returned to the client for further use.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | Creates a stream for a specific page preview |
| releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | Notifies that the page preview generation is done and gets the output stream. |

### getWidth() {#getWidth--}
```
public int getWidth()
```


Gets the page preview width.

**Returns:**
int - The page width.
### setWidth(int width) {#setWidth-int-}
```
public void setWidth(int width)
```


Sets the page preview width.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| width | int | The page width. |

### getHeight() {#getHeight--}
```
public int getHeight()
```


Gets the page preview height.

**Returns:**
int - The page height.
### setHeight(int height) {#setHeight-int-}
```
public void setHeight(int height)
```


Sets the page preview height.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| height | int | The page height. |

### getDpi() {#getDpi--}
```
public int getDpi()
```


Gets a dpi.

**Returns:**
int - An integer value that represents a dpi.
### setDpi(int dpi) {#setDpi-int-}
```
public void setDpi(int dpi)
```


Sets a dpi.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dpi | int | The dpi. |

### getPageNumbers() {#getPageNumbers--}
```
public int[] getPageNumbers()
```


Gets an array of page numbers to generate previews.

**Returns:**
int[] - A collection of page numbers.
### setPageNumbers(int[] pageNumbers) {#setPageNumbers-int---}
```
public void setPageNumbers(int[] pageNumbers)
```


Sets an array of page numbers to generate previews.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageNumbers | int[] | A collection of page numbers. |

### getPreviewFormat() {#getPreviewFormat--}
```
public PreviewFormats getPreviewFormat()
```


Gets the preview image format.

**Returns:**
[PreviewFormats](../../com.groupdocs.parser.options/previewformats) - [PreviewFormats](../../com.groupdocs.parser.options/previewformats) numeration.
### setPreviewFormat(PreviewFormats previewFormat) {#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-}
```
public void setPreviewFormat(PreviewFormats previewFormat)
```


Sets the preview image format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| previewFormat | [PreviewFormats](../../com.groupdocs.parser.options/previewformats) | The preview format. |

### getCreatePageStream() {#getCreatePageStream--}
```
public ICreatePageStream getCreatePageStream()
```


Gets an instance of the page stream creation delegate.

**Returns:**
[ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) - The page stream creation delegate.
### setCreatePageStream(ICreatePageStream createPageStream) {#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-}
```
public void setCreatePageStream(ICreatePageStream createPageStream)
```


Sets an instance of the page stream creation delegate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | The page stream creation delegate. |

### getReleasePageStream() {#getReleasePageStream--}
```
public IReleasePageStream getReleasePageStream()
```


Gets an instance of the page preview completion delegate.

**Returns:**
[IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) - The page preview completion delegate.
### setReleasePageStream(IReleasePageStream releasePageStream) {#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public void setReleasePageStream(IReleasePageStream releasePageStream)
```


Sets an instance of the page preview completion delegate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | The page preview completion delegate. |

### getPreviewPageRender() {#getPreviewPageRender--}
```
public IPreviewPageRender getPreviewPageRender()
```


Gets an instance of the page preview render info delegate.

**Returns:**
[IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) - The page preview render info delegate.
### setPreviewPageRender(IPreviewPageRender previewPageRender) {#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-}
```
public void setPreviewPageRender(IPreviewPageRender previewPageRender)
```


Sets an instance of the page preview render info delegate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| previewPageRender | [IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) | The page preview render info delegate. |

