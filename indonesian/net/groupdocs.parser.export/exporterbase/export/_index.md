---
title: "Ekspor"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mengekspor koleksi metadata ke aliran."
type: docs
weight: 10
url: /id/net/groupdocs.parser.export/exporterbase/export/
---

## Export(IEnumerable&lt;MetadataItem&gt;, Stream) {#export_4}

Mengekspor koleksi metadata ke aliran.

```csharp
public abstract void Export(IEnumerable<MetadataItem> metadata, Stream stream)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| metadata | IEnumerable`1 | Koleksi metadata. |
| stream | Stream | Aliran output. |

### Lihat Juga

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;MetadataItem&gt;, string) {#export_5}

Mengekspor koleksi metadata ke file.

```csharp
public void Export(IEnumerable<MetadataItem> metadata, string fileName)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| metadata | IEnumerable`1 | Koleksi metadata. |
| fileName | String | Jalur lengkap ke file output. |

### Lihat Juga

* class [MetadataItem](../../../groupdocs.parser.data/metadataitem)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, Stream) {#export_2}

Mengekspor informasi dokumen ke aliran.

```csharp
public abstract void Export(IDocumentInfo documentInfo, Stream stream)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| documentInfo | IDocumentInfo | Informasi dokumen. |
| stream | Stream | Aliran output. |

### Lihat Juga

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IDocumentInfo, string) {#export_3}

Mengekspor informasi dokumen ke file.

```csharp
public void Export(IDocumentInfo documentInfo, string fileName)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| documentInfo | IDocumentInfo | Informasi dokumen. |
| fileName | String | Jalur lengkap ke file output. |

### Lihat Juga

* interface [IDocumentInfo](../../../groupdocs.parser.options/idocumentinfo)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, Stream) {#export_10}

Mengekspor koleksi area teks ke aliran.

```csharp
public abstract void Export(IEnumerable<PageTextArea> textAreas, Stream stream)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| textAreas | IEnumerable`1 | Koleksi area teks. |
| stream | Stream | Aliran output. |

### Lihat Juga

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTextArea&gt;, string) {#export_11}

Mengekspor koleksi area teks ke file.

```csharp
public void Export(IEnumerable<PageTextArea> textAreas, string fileName)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| textAreas | IEnumerable`1 | Koleksi area teks. |
| fileName | String | Jalur lengkap ke file output. |

### Lihat Juga

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, Stream) {#export_8}

Mengekspor koleksi tabel ke aliran.

```csharp
public abstract void Export(IEnumerable<PageTableArea> tables, Stream stream)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| tables | IEnumerable`1 | Koleksi tabel. |
| stream | Stream | Aliran output. |

### Lihat Juga

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageTableArea&gt;, string) {#export_9}

Mengekspor koleksi tabel ke file.

```csharp
public void Export(IEnumerable<PageTableArea> tables, string fileName)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| tables | IEnumerable`1 | Koleksi tabel. |
| fileName | String | Jalur lengkap ke file output. |

### Lihat Juga

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, Stream) {#export_6}

Mengekspor koleksi kode batang ke aliran.

```csharp
public abstract void Export(IEnumerable<PageBarcodeArea> barcodes, Stream stream)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| barcodes | IEnumerable`1 | Koleksi kode batang. |
| stream | Stream | Aliran output. |

### Lihat Juga

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(IEnumerable&lt;PageBarcodeArea&gt;, string) {#export_7}

Mengekspor koleksi kode batang ke file.

```csharp
public void Export(IEnumerable<PageBarcodeArea> barcodes, string fileName)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| barcodes | IEnumerable`1 | Koleksi kode batang. |
| fileName | String | Jalur lengkap ke file output. |

### Lihat Juga

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, Stream) {#export}

Mengekspor data dokumen ke aliran.

```csharp
public abstract void Export(DocumentData documentData, Stream stream)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| documentData | DocumentData | Data dokumen. |
| stream | Stream | Aliran output. |

### Lihat Juga

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

---

## Export(DocumentData, string) {#export_1}

Mengekspor data dokumen ke file.

```csharp
public void Export(DocumentData documentData, string fileName)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| documentData | DocumentData | Data dokumen. |
| fileName | String | Jalur lengkap ke file output. |

### Lihat Juga

* class [DocumentData](../../../groupdocs.parser.data/documentdata)
* class [ExporterBase](../../exporterbase)
* namespace [GroupDocs.Parser.Export](../../../groupdocs.parser.export)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
