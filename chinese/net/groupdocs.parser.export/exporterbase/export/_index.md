---
title: "导出"
second_title: "GroupDocs.Parser for .NET API 参考"
description: "将元数据集合导出到流。"
type: docs
weight: 10
url: /zh/net/groupdocs.parser.export/exporterbase/export/
---

## Export(IEnumerable&lt;MetadataItem&gt;, Stream) {#export_4}

将元数据集合导出到流。

```csharp
public abstract void Export(IEnumerable<MetadataItem> metadata, Stream stream)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 元数据 | IEnumerable`1 | 元数据的集合。 |
| 流 | Stream | 输出流。 |

### 另请参见

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;MetadataItem&gt;, string) {#export_5}

将元数据集合导出到文件。

```csharp
public void Export(IEnumerable<MetadataItem> metadata, string fileName)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 元数据 | IEnumerable`1 | 元数据的集合。 |
| 文件名 | 字符串 | 输出文件的完整路径。 |

### 另请参见

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, Stream) {#export_2}

将文档信息导出到流。

```csharp
public abstract void Export(IDocumentInfo documentInfo, Stream stream)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 文档信息 | IDocumentInfo | 文档信息。 |
| 流 | Stream | 输出流。 |

### 另请参见

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, string) {#export_3}

将文档信息导出到文件。

```csharp
public void Export(IDocumentInfo documentInfo, string fileName)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 文档信息 | IDocumentInfo | 文档信息。 |
| 文件名 | 字符串 | 输出文件的完整路径。 |

### 另请参见

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, Stream) {#export_10}

将文本区域集合导出到流。

```csharp
public abstract void Export(IEnumerable<PageTextArea> textAreas, Stream stream)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 文本区域 | IEnumerable`1 | 文本区域的集合。 |
| 流 | Stream | 输出流。 |

### 另请参见

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, string) {#export_11}

将文本区域集合导出到文件。

```csharp
public void Export(IEnumerable<PageTextArea> textAreas, string fileName)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 文本区域 | IEnumerable`1 | 文本区域的集合。 |
| 文件名 | 字符串 | 输出文件的完整路径。 |

### 另请参见

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, Stream) {#export_8}

将表格集合导出到流。

```csharp
public abstract void Export(IEnumerable<PageTableArea> tables, Stream stream)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 表格 | IEnumerable`1 | 表格的集合。 |
| 流 | Stream | 输出流。 |

### 另请参见

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, string) {#export_9}

将表格集合导出到文件。

```csharp
public void Export(IEnumerable<PageTableArea> tables, string fileName)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 表格 | IEnumerable`1 | 表格的集合。 |
| 文件名 | 字符串 | 输出文件的完整路径。 |

### 另请参见

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, Stream) {#export_6}

将条码集合导出到流。

```csharp
public abstract void Export(IEnumerable<PageBarcodeArea> barcodes, Stream stream)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 条形码 | IEnumerable`1 | 条形码的集合。 |
| 流 | Stream | 输出流。 |

### 另请参见

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, string) {#export_7}

将条码集合导出到文件。

```csharp
public void Export(IEnumerable<PageBarcodeArea> barcodes, string fileName)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 条形码 | IEnumerable`1 | 条形码的集合。 |
| 文件名 | 字符串 | 输出文件的完整路径。 |

### 另请参见

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, Stream) {#export}

将文档数据导出到流。

```csharp
public abstract void Export(DocumentData documentData, Stream stream)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 文档数据 | DocumentData | 文档数据。 |
| 流 | Stream | 输出流。 |

### 另请参见

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, string) {#export_1}

将文档数据导出到文件。

```csharp
public void Export(DocumentData documentData, string fileName)
```

| Parameter | Type | 描述 |
| --- | --- | --- |
| 文档数据 | DocumentData | 文档数据。 |
| 文件名 | 字符串 | 输出文件的完整路径。 |

### 另请参见

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
