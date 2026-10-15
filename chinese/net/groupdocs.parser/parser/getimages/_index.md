---
title: "GetImages"
second_title: "GroupDocs.Parser for .NET API 参考"
description: "从文档中提取图像。"
type: docs
weight: 130
url: /zh/net/groupdocs.parser/parser/getimages/
---

## GetImages() {#getimages}

从文档中提取图像。

```csharp
public IEnumerable<PageImageArea> GetImages()
```

### 返回值

一组 [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) 对象；如果不支持图像提取，则为 `null`。

### 备注

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### 示例

以下示例展示如何从整个文档中提取所有图像：

```csharp
// 创建 Parser 类的实例
using (Parser parser = new Parser(filePath))
{
    // 提取图像
    IEnumerable<PageImageArea> images = parser.GetImages();
    // 检查是否支持图像提取
    if (images == null)
    {
        Console.WriteLine("Images extraction isn't supported");
        return;
    }
    // 遍历图像
    foreach (PageImageArea image in images)
    {
        // 打印页面索引、矩形和图像类型：
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### 另请参见

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(PageAreaOptions) {#getimages_1}

使用自定义选项从文档中提取图像（用于设置包含图像的矩形区域）。

```csharp
public IEnumerable<PageImageArea> GetImages(PageAreaOptions options)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| options | PageAreaOptions | 图像提取选项。 |

### 返回值

一组 [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) 对象；如果不支持图像提取，则为 `null`。

### 备注

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from document page area](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### 示例

以下示例展示如何仅从左上角提取图像：

```csharp
// 创建 Parser 类的实例
using (Parser parser = new Parser(filePath))
{
    // 创建用于图像提取的选项
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(0, 0), new Size(300, 100)));
    // 从页面的左上角提取图像：
    IEnumerable<PageImageArea> images = parser.GetImages(options);
    // 检查是否支持图像提取
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }
    // 遍历图像
    foreach (PageImageArea image in images)
    {
        // 打印页面索引、矩形和图像类型：
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### 另请参见

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(int) {#getimages_2}

从文档页面中提取图像。

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| pageIndex | Int32 | 基于零的页面索引。 |

### 返回值

一组 [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) 对象；如果不支持图像提取，则为 `null`。

### 备注

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from document page](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### 示例

要从文档页面提取图像，使用以下方法：

```csharp
// 创建 Parser 类的实例
using (Parser parser = new Parser(filePath))
{
    // 检查文档是否支持图像提取
    if (!parser.Features.Images)
    {
        Console.WriteLine("Document isn't supports images extraction.");
        return;
    }
    
    // 获取文档信息
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // 检查文档是否有页面
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // 遍历页面
    for (int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // 打印页面编号 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // 遍历图像
        // 我们忽略空值检查，因为我们已提前检查过图像提取功能的支持情况
        foreach (PageImageArea image in parser.GetImages(pageIndex))
        {
            // 打印矩形和图像类型
            Console.WriteLine(string.Format("R: {0}, Text: {1}", image.Rectangle, image.FileType));
        }
    }
}
```

### 另请参见

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(int, PageAreaOptions) {#getimages_3}

使用自定义选项从文档页面中提取图像（用于设置包含图像的矩形区域）。

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex, PageAreaOptions options)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| pageIndex | Int32 | 基于零的页面索引。 |
| options | PageAreaOptions | 图像提取选项。 |

### 返回值

一组 [`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) 对象；如果不支持图像提取，则为 `null`。

### 备注

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from document page](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extract images from document page area](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### 另请参见

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
