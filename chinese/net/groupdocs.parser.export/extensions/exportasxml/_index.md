---
title: "ExportAsXml"
second_title: "GroupDocs.Parser for .NET API 参考"
description: "以 XML 格式将元数据集合导出到流中。"
type: docs
weight: 20
url: /zh/net/groupdocs.parser.export/extensions/exportasxml/
---

## ExportAsXml(this IEnumerable&lt;MetadataItem&gt;, Stream) {#exportasxml_4}

以 XML 格式将元数据集合导出到流中。

```csharp
public static void ExportAsXml(this IEnumerable<MetadataItem> metadata, Stream stream)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 元数据 | IEnumerable`1 | 元数据的集合。 |
| 流 | Stream | 输出流。 |

### 另请参见

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;MetadataItem&gt;, string) {#exportasxml_5}

以 XML 格式将元数据集合导出到文件中。

```csharp
public static void ExportAsXml(this IEnumerable<MetadataItem> metadata, string fileName)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 元数据 | IEnumerable`1 | 元数据的集合。 |
| 文件名 | 字符串 | 输出文件的完整路径。 |

### 另请参见

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IDocumentInfo, Stream) {#exportasxml_2}

以 XML 格式将文档信息导出到流中。

```csharp
public static void ExportAsXml(this IDocumentInfo documentInfo, Stream stream)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 文档信息 | IDocumentInfo | 文档信息。 |
| 流 | Stream | 输出流。 |

### 另请参见

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IDocumentInfo, string) {#exportasxml_3}

以 XML 格式将文档信息导出到文件中。

```csharp
public static void ExportAsXml(this IDocumentInfo documentInfo, string fileName)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 文档信息 | IDocumentInfo | 文档信息。 |
| 文件名 | 字符串 | 输出文件的完整路径。 |

### 另请参见

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;PageTextArea&gt;, Stream) {#exportasxml_10}

以 XML 格式将文本区域集合导出到流中。

```csharp
public static void ExportAsXml(this IEnumerable<PageTextArea> textAreas, Stream stream)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 文本区域 | IEnumerable`1 | 文本区域的集合。 |
| 流 | Stream | 输出流。 |

### 另请参见

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;PageTextArea&gt;, string) {#exportasxml_11}

以 XML 格式将文本区域的 collectiob 导出到文件中。

```csharp
public static void ExportAsXml(this IEnumerable<PageTextArea> textAreas, string fileName)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 文本区域 | IEnumerable`1 | 文本区域的集合。 |
| 文件名 | 字符串 | 输出文件的完整路径。 |

### 另请参见

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;PageTableArea&gt;, Stream) {#exportasxml_8}

以 XML 格式将表格集合导出到流中。

```csharp
public static void ExportAsXml(this IEnumerable<PageTableArea> tables, Stream stream)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 表格 | IEnumerable`1 | 表格的集合。 |
| 流 | Stream | 输出流。 |

### 另请参见

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;PageTableArea&gt;, string) {#exportasxml_9}

以 XML 格式将表格集合导出到文件中。

```csharp
public static void ExportAsXml(this IEnumerable<PageTableArea> tables, string fileName)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 表格 | IEnumerable`1 | 表格的集合。 |
| 文件名 | 字符串 | 输出文件的完整路径。 |

### 另请参见

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;PageBarcodeArea&gt;, Stream) {#exportasxml_6}

以 XML 格式将条形码集合导出到流中。

```csharp
public static void ExportAsXml(this IEnumerable<PageBarcodeArea> barcodes, Stream stream)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 条形码 | IEnumerable`1 | 条形码的集合。 |
| 流 | Stream | 输出流。 |

### 另请参见

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this IEnumerable&lt;PageBarcodeArea&gt;, string) {#exportasxml_7}

以 XML 格式将条形码集合导出到文件中。

```csharp
public static void ExportAsXml(this IEnumerable<PageBarcodeArea> barcodes, string fileName)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 条形码 | IEnumerable`1 | 条形码的集合。 |
| 文件名 | 字符串 | 输出文件的完整路径。 |

### 另请参见

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this DocumentData, Stream) {#exportasxml}

以 XML 格式将文档数据导出到流中。

```csharp
public static void ExportAsXml(this DocumentData documentData, Stream stream)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 文档数据 | DocumentData | 文档数据。 |
| 流 | Stream | 输出流。 |

### 另请参见

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## ExportAsXml(this DocumentData, string) {#exportasxml_1}

以 XML 格式将文档数据导出到文件中。

```csharp
public static void ExportAsXml(this DocumentData documentData, string fileName)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 文档数据 | DocumentData | 文档数据。 |
| 文件名 | 字符串 | 输出文件的完整路径。 |

### 另请参见

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [Extensions](../../extensions)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
