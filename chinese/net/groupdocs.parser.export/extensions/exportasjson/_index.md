---
title: "ExportAsJson"
second_title: "GroupDocs.Parser for .NET API 参考"
description: "以 JSON 格式将元数据集合导出到流中。"
type: docs
weight: 10
url: /zh/net/groupdocs.parser.export/extensions/exportasjson/
---

## ExportAsJson(this IEnumerable&lt;MetadataItem&gt;, Stream) {#exportasjson_4}

以 JSON 格式将元数据集合导出到流中。

```csharp
public static void ExportAsJson(this IEnumerable<MetadataItem> metadata, Stream stream)
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

## ExportAsJson(this IEnumerable&lt;MetadataItem&gt;, string) {#exportasjson_5}

以 JSON 格式将元数据集合导出到文件中。

```csharp
public static void ExportAsJson(this IEnumerable<MetadataItem> metadata, string fileName)
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

## ExportAsJson(this IDocumentInfo, Stream) {#exportasjson_2}

以 JSON 格式将文档信息导出到流中。

```csharp
public static void ExportAsJson(this IDocumentInfo documentInfo, Stream stream)
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

## ExportAsJson(this IDocumentInfo, string) {#exportasjson_3}

以 JSON 格式将文档信息导出到文件中。

```csharp
public static void ExportAsJson(this IDocumentInfo documentInfo, string fileName)
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

## ExportAsJson(this IEnumerable&lt;PageTextArea&gt;, Stream) {#exportasjson_10}

以 JSON 格式将文本区域集合导出到流中。

```csharp
public static void ExportAsJson(this IEnumerable<PageTextArea> textAreas, Stream stream)
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

## ExportAsJson(this IEnumerable&lt;PageTextArea&gt;, string) {#exportasjson_11}

以 JSON 格式将文本区域的 collectiob 导出到文件中。

```csharp
public static void ExportAsJson(this IEnumerable<PageTextArea> textAreas, string fileName)
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

## ExportAsJson(this IEnumerable&lt;PageTableArea&gt;, Stream) {#exportasjson_8}

以 JSON 格式将表格集合导出到流中。

```csharp
public static void ExportAsJson(this IEnumerable<PageTableArea> tables, Stream stream)
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

## ExportAsJson(this IEnumerable&lt;PageTableArea&gt;, string) {#exportasjson_9}

以 JSON 格式将表格集合导出到文件中。

```csharp
public static void ExportAsJson(this IEnumerable<PageTableArea> tables, string fileName)
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

## ExportAsJson(this IEnumerable&lt;PageBarcodeArea&gt;, Stream) {#exportasjson_6}

以 JSON 格式将条形码集合导出到流中。

```csharp
public static void ExportAsJson(this IEnumerable<PageBarcodeArea> barcodes, Stream stream)
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

## ExportAsJson(this IEnumerable&lt;PageBarcodeArea&gt;, string) {#exportasjson_7}

以 JSON 格式将条形码集合导出到文件中。

```csharp
public static void ExportAsJson(this IEnumerable<PageBarcodeArea> barcodes, string fileName)
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

## ExportAsJson(this DocumentData, Stream) {#exportasjson}

将文档数据以 JSON 格式导出到流。

```csharp
public static void ExportAsJson(this DocumentData documentData, Stream stream)
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

## ExportAsJson(this DocumentData, string) {#exportasjson_1}

将文档数据以 JSON 格式导出到文件。

```csharp
public static void ExportAsJson(this DocumentData documentData, string fileName)
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
