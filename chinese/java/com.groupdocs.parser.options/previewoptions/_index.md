---
title: "PreviewOptions"
second_title: "GroupDocs.Parser 用于 Java 的 API 参考"
description: "提供用于设置预览生成的需求和流委托的选项。"
type: docs
weight: 34
url: /zh/java/com.groupdocs.parser.options/previewoptions/
---
**Inheritance:**
java.lang.Object
```
public class PreviewOptions
```

提供用于设置预览生成的需求和流委托的选项。

## 构造函数

| 构造函数 | 描述 |
| --- | --- |
|  | [PreviewOptions(ICreatePageStream createPageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-) | 初始化 [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) 类的新实例，使输出流被关闭。 |
|
|  | [PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)](#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-) | 初始化 [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) 类的新实例，使输出流返回给客户端以供进一步使用。 |
|
## 方法

| 方法 | 描述 |
| --- | --- |
|  | [getWidth()](#getWidth--) | 获取页面预览宽度。 |
|
|  | [setWidth(int width)](#setWidth-int-) | 设置页面预览宽度。 |
|
|  | [getHeight()](#getHeight--) | 获取页面预览高度。 |
|
|  | [setHeight(int height)](#setHeight-int-) | 设置页面预览高度。 |
|
|  | [getDpi()](#getDpi--) | 获取 DPI。 |
|
|  | [setDpi(int dpi)](#setDpi-int-) | 设置 DPI。 |
|
|  | [getPageNumbers()](#getPageNumbers--) | 获取用于生成预览的页面编号数组。 |
|
|  | [setPageNumbers(int[] pageNumbers)](#setPageNumbers-int---) | 设置用于生成预览的页面编号数组。 |
|
|  | [getPreviewFormat()](#getPreviewFormat--) | 获取预览图像格式。 |
|
|  | [setPreviewFormat(PreviewFormats previewFormat)](#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-) | 设置预览图像格式。 |
|
|  | [getCreatePageStream()](#getCreatePageStream--) | 获取页面流创建委托的实例。 |
|
|  | [setCreatePageStream(ICreatePageStream createPageStream)](#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-) | 设置页面流创建委托的实例。 |
|
|  | [getReleasePageStream()](#getReleasePageStream--) | 获取页面预览完成委托的实例。 |
|
|  | [setReleasePageStream(IReleasePageStream releasePageStream)](#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-) | 设置页面预览完成委托的实例。 |
|
|  | [getPreviewPageRender()](#getPreviewPageRender--) | 获取页面预览渲染信息委托的实例。 |
|
|  | [setPreviewPageRender(IPreviewPageRender previewPageRender)](#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-) | 设置页面预览渲染信息委托的实例。 |
|
### PreviewOptions(ICreatePageStream createPageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream)
```


初始化 [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) 类的新实例，使输出流被关闭。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | 为特定页面预览创建流。 |
|

### PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream) {#PreviewOptions-com.groupdocs.parser.options.ICreatePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public PreviewOptions(ICreatePageStream createPageStream, IReleasePageStream releasePageStream)
```


初始化 [PreviewOptions](../../com.groupdocs.parser.options/previewoptions) 类的新实例，使输出流返回给客户端以供进一步使用。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | 为特定页面预览创建流 |
|
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | 通知页面预览生成完成并获取输出流。 |
|

### getWidth() {#getWidth--}
```
public int getWidth()
```


获取页面预览宽度。


**Returns:**
int - 页面宽度。

### setWidth(int width) {#setWidth-int-}
```
public void setWidth(int width)
```


设置页面预览宽度。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 宽度 | int | 页面宽度。 |
|

### getHeight() {#getHeight--}
```
public int getHeight()
```


获取页面预览高度。


**Returns:**
int - 页面高度。

### setHeight(int height) {#setHeight-int-}
```
public void setHeight(int height)
```


设置页面预览高度。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | 高度 | int | 页面高度。 |
|

### getDpi() {#getDpi--}
```
public int getDpi()
```


获取 DPI。


**Returns:**
int - 表示 DPI 的整数值。

### setDpi(int dpi) {#setDpi-int-}
```
public void setDpi(int dpi)
```


设置 DPI。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | DPI | int | 每英寸点数。 |
|

### getPageNumbers() {#getPageNumbers--}
```
public int[] getPageNumbers()
```


获取用于生成预览的页面编号数组。


**Returns:**
int[] - 页面编号的集合。

### setPageNumbers(int[] pageNumbers) {#setPageNumbers-int---}
```
public void setPageNumbers(int[] pageNumbers)
```


设置用于生成预览的页面编号数组。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | pageNumbers | int[] | 页面编号的集合。 |
|

### getPreviewFormat() {#getPreviewFormat--}
```
public PreviewFormats getPreviewFormat()
```


获取预览图像格式。


**Returns:**
[PreviewFormats](../../com.groupdocs.parser.options/previewformats) - [PreviewFormats](../../com.groupdocs.parser.options/previewformats) numeration.

### setPreviewFormat(PreviewFormats previewFormat) {#setPreviewFormat-com.groupdocs.parser.options.PreviewFormats-}
```
public void setPreviewFormat(PreviewFormats previewFormat)
```


设置预览图像格式。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | previewFormat | [PreviewFormats](../../com.groupdocs.parser.options/previewformats) | 预览格式。 |
|

### getCreatePageStream() {#getCreatePageStream--}
```
public ICreatePageStream getCreatePageStream()
```


获取页面流创建委托的实例。


**Returns:**
[ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) - The page stream creation delegate.

### setCreatePageStream(ICreatePageStream createPageStream) {#setCreatePageStream-com.groupdocs.parser.options.ICreatePageStream-}
```
public void setCreatePageStream(ICreatePageStream createPageStream)
```


设置页面流创建委托的实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | createPageStream | [ICreatePageStream](../../com.groupdocs.parser.options/icreatepagestream) | 页面流创建委托。 |
|

### getReleasePageStream() {#getReleasePageStream--}
```
public IReleasePageStream getReleasePageStream()
```


获取页面预览完成委托的实例。


**Returns:**
[IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) - The page preview completion delegate.

### setReleasePageStream(IReleasePageStream releasePageStream) {#setReleasePageStream-com.groupdocs.parser.options.IReleasePageStream-}
```
public void setReleasePageStream(IReleasePageStream releasePageStream)
```


设置页面预览完成委托的实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | releasePageStream | [IReleasePageStream](../../com.groupdocs.parser.options/ireleasepagestream) | 页面预览完成委托。 |
|

### getPreviewPageRender() {#getPreviewPageRender--}
```
public IPreviewPageRender getPreviewPageRender()
```


获取页面预览渲染信息委托的实例。


**Returns:**
[IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) - The page preview render info delegate.

### setPreviewPageRender(IPreviewPageRender previewPageRender) {#setPreviewPageRender-com.groupdocs.parser.options.IPreviewPageRender-}
```
public void setPreviewPageRender(IPreviewPageRender previewPageRender)
```


设置页面预览渲染信息委托的实例。


**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | previewPageRender | [IPreviewPageRender](../../com.groupdocs.parser.options/ipreviewpagerender) | 页面预览渲染信息委托。 |
|

