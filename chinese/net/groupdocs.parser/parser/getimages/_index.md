---
title: GetImages
second_title: GroupDocs.Parser for .NET API 参考
description: 从文档中提取图像
type: docs
weight: 110
url: /zh/net/groupdocs.parser/parser/getimages/
---
## GetImages() {#getimages}

从文档中提取图像。

```csharp
public IEnumerable<PageImageArea> GetImages()
```

### 返回值

的集合[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea)对象； `无效的`如果不支持图像提取.

### 评论

**了解更多：**

* [从文档中提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [将图像提取到文件](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [从 Microsoft Office Word 文档中提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [从 Microsoft Office Excel 电子表格中提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [从 Microsoft Office PowerPoint 演示文稿中提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [从电子邮件中提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [从 PDF 文档中提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### 例子

以下示例显示了如何从整个文档中提取所有图像：

```csharp
// 创建解析器类的实例
using (Parser parser = new Parser(filePath))
{
    // 提取图像
    IEnumerable<PageImageArea> images = parser.GetImages();
    // 检查是否支持图片提取
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

### 也可以看看

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* 命名空间 [GroupDocs.Parser](../../parser)
* 部件 [GroupDocs.Parser](../../../)

---

## GetImages(PageAreaOptions) {#getimages_1}

使用自定义选项从文档中提取图像 （设置包含图像的矩形区域）。

```csharp
public IEnumerable<PageImageArea> GetImages(PageAreaOptions options)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| options | PageAreaOptions | 图像提取的选项。 |

### 返回值

的集合[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea)对象； `无效的`如果不支持图像提取.

### 评论

**了解更多：**

* [从文档中提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [将图像提取到文件](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [从文档页面区域提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [从 Microsoft Office Word 文档中提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [从 Microsoft Office Excel 电子表格中提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [从 Microsoft Office PowerPoint 演示文稿中提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [从电子邮件中提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [从 PDF 文档中提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### 例子

以下示例显示如何仅从左上角提取图像：

```csharp
// 创建解析器类的实例
using (Parser parser = new Parser(filePath))
{
    // 创建用于图像提取的选项
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(0, 0), new Size(300, 100)));
    // 从页面的左上角提取图像：
    IEnumerable<PageImageArea> images = parser.GetImages(options);
    // 检查是否支持图片提取
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

### 也可以看看

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* 命名空间 [GroupDocs.Parser](../../parser)
* 部件 [GroupDocs.Parser](../../../)

---

## GetImages(int) {#getimages_2}

从文档页面中提取图像。

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| pageIndex | Int32 | 从零开始的页面索引。 |

### 返回值

的集合[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea)对象； `无效的`如果不支持图像提取.

### 评论

**了解更多：**

* [从文档中提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [将图像提取到文件](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [从文档页面中提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [从 Microsoft Office Word 文档中提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [从 Microsoft Office Excel 电子表格中提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [从 Microsoft Office PowerPoint 演示文稿中提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [从电子邮件中提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [从 PDF 文档中提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### 例子

要从文档页面中提取图像，使用以下方法：

```csharp
// 创建解析器类的实例
using (Parser parser = new Parser(filePath))
{
    // 检查文档是否支持图片提取
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
        // 打印页码 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // 遍历图像
        // 我们忽略空值检查，因为我们之前已经检查过图像提取功能支持
        foreach (PageImageArea image in parser.GetImages(pageIndex))
        {
            // 打印矩形和图像类型
            Console.WriteLine(string.Format("R: {0}, Text: {1}", image.Rectangle, image.FileType));
        }
    }
}
```

### 也可以看看

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* 命名空间 [GroupDocs.Parser](../../parser)
* 部件 [GroupDocs.Parser](../../../)

---

## GetImages(int, PageAreaOptions) {#getimages_3}

使用自定义选项从文档页面中提取图像 （设置包含图像的矩形区域）。

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex, PageAreaOptions options)
```

| 范围 | 类型 | 描述 |
| --- | --- | --- |
| pageIndex | Int32 | 从零开始的页面索引。 |
| options | PageAreaOptions | 图像提取的选项。 |

### 返回值

的集合[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea)对象； `无效的`如果不支持图像提取.

### 评论

**了解更多：**

* [从文档中提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [将图像提取到文件](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [从文档页面中提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [从文档页面区域提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [从 Microsoft Office Word 文档中提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [从 Microsoft Office Excel 电子表格中提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [从 Microsoft Office PowerPoint 演示文稿中提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [从电子邮件中提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [从 PDF 文档中提取图像](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### 也可以看看

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* 命名空间 [GroupDocs.Parser](../../parser)
* 部件 [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
