---
title: "تصدير"
second_title: "GroupDocs.Parser لـ .NET API مرجع"
description: "يصدّر مجموعة البيانات الوصفية إلى التدفق."
type: docs
weight: 10
url: /ar/net/groupdocs.parser.export/exporterbase/export/
---

## Export(IEnumerable&lt;MetadataItem&gt;, Stream) {#export_4}

يصدّر مجموعة البيانات الوصفية إلى التدفق.

```csharp
public abstract void Export(IEnumerable<MetadataItem> metadata, Stream stream)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| البيانات الوصفية | IEnumerable`1 | مجموعة البيانات الوصفية. |
| تدفق | Stream | تدفق الإخراج. |

### انظر أيضًا

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;MetadataItem&gt;, string) {#export_5}

يصدّر مجموعة البيانات الوصفية إلى الملف.

```csharp
public void Export(IEnumerable<MetadataItem> metadata, string fileName)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| البيانات الوصفية | IEnumerable`1 | مجموعة البيانات الوصفية. |
| fileName | سلسلة | المسار الكامل إلى ملف الإخراج. |

### انظر أيضًا

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, Stream) {#export_2}

يصدّر معلومات المستند إلى التدفق.

```csharp
public abstract void Export(IDocumentInfo documentInfo, Stream stream)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| documentInfo | IDocumentInfo | معلومات المستند. |
| تدفق | Stream | تدفق الإخراج. |

### انظر أيضًا

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, string) {#export_3}

يصدّر معلومات المستند إلى الملف.

```csharp
public void Export(IDocumentInfo documentInfo, string fileName)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| documentInfo | IDocumentInfo | معلومات المستند. |
| fileName | سلسلة | المسار الكامل إلى ملف الإخراج. |

### انظر أيضًا

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, Stream) {#export_10}

يصدّر مجموعة مناطق النص إلى التدفق.

```csharp
public abstract void Export(IEnumerable<PageTextArea> textAreas, Stream stream)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| textAreas | IEnumerable`1 | مجموعة مناطق النص. |
| تدفق | Stream | تدفق الإخراج. |

### انظر أيضًا

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, string) {#export_11}

يصدّر مجموعة مناطق النص إلى الملف.

```csharp
public void Export(IEnumerable<PageTextArea> textAreas, string fileName)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| textAreas | IEnumerable`1 | مجموعة مناطق النص. |
| fileName | سلسلة | المسار الكامل إلى ملف الإخراج. |

### انظر أيضًا

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, Stream) {#export_8}

يصدّر مجموعة الجداول إلى التدفق.

```csharp
public abstract void Export(IEnumerable<PageTableArea> tables, Stream stream)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| الجداول | IEnumerable`1 | مجموعة الجداول. |
| تدفق | Stream | تدفق الإخراج. |

### انظر أيضًا

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, string) {#export_9}

يصدّر مجموعة الجداول إلى الملف.

```csharp
public void Export(IEnumerable<PageTableArea> tables, string fileName)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| الجداول | IEnumerable`1 | مجموعة الجداول. |
| fileName | سلسلة | المسار الكامل إلى ملف الإخراج. |

### انظر أيضًا

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, Stream) {#export_6}

يصدّر مجموعة الباركودات إلى التدفق.

```csharp
public abstract void Export(IEnumerable<PageBarcodeArea> barcodes, Stream stream)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| الباركودات | IEnumerable`1 | مجموعة الباركود. |
| تدفق | Stream | تدفق الإخراج. |

### انظر أيضًا

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, string) {#export_7}

يصدّر مجموعة الباركودات إلى الملف.

```csharp
public void Export(IEnumerable<PageBarcodeArea> barcodes, string fileName)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| الباركودات | IEnumerable`1 | مجموعة الباركود. |
| fileName | سلسلة | المسار الكامل إلى ملف الإخراج. |

### انظر أيضًا

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, Stream) {#export}

يصدّر بيانات المستند إلى التدفق.

```csharp
public abstract void Export(DocumentData documentData, Stream stream)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| documentData | DocumentData | بيانات المستند. |
| تدفق | Stream | تدفق الإخراج. |

### انظر أيضًا

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, string) {#export_1}

يصدّر بيانات المستند إلى الملف.

```csharp
public void Export(DocumentData documentData, string fileName)
```

| Parameter | Type | الوصف |
| --- | --- | --- |
| documentData | DocumentData | بيانات المستند. |
| fileName | سلسلة | المسار الكامل إلى ملف الإخراج. |

### انظر أيضًا

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
