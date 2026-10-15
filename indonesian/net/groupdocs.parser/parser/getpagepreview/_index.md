---
title: "GetPagePreview"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menghasilkan pratinjau halaman dokumen."
type: docs
weight: 150
url: /id/net/groupdocs.parser/parser/getpagepreview/
---

## GetPagePreview(int) {#getpagepreview}

Menghasilkan pratinjau halaman dokumen.

```csharp
public Stream GetPagePreview(int pageIndex)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| pageIndex | Int32 | Indeks halaman berbasis nol. |

### Nilai Kembali

Sebuah instance dari Stream yang berisi gambar halaman dokumen; `null` jika pembuatan pratinjau halaman tidak didukung.

### Lihat Juga

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetPagePreview(int, PagePreviewOptions) {#getpagepreview_1}

Menghasilkan pratinjau halaman dokumen menggunakan opsi penyesuaian.

```csharp
public Stream GetPagePreview(int pageIndex, PagePreviewOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| pageIndex | Int32 | Indeks halaman berbasis nol. |
| options | PagePreviewOptions | Opsi untuk menyesuaikan pembuatan pratinjau. |

### Nilai Kembali

Sebuah instance dari Stream yang berisi gambar halaman dokumen; `null` jika pembuatan pratinjau halaman tidak didukung.

### Lihat Juga

* class [PagePreviewOptions](../../../groupdocs.parser.options/pagepreviewoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
