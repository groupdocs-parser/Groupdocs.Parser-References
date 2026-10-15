---
title: "GetAnnotations"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mengekstrak anotasi dari dokumen. Perhatikan bahwa hanya format PDF yang saat ini didukung."
type: docs
weight: 60
url: /id/net/groupdocs.parser/parser/getannotations/
---

## GetAnnotations() {#getannotations}

Mengekstrak anotasi dari dokumen. Perhatikan bahwa hanya format PDF yang saat ini didukung.

```csharp
public IEnumerable<AnnotationItem> GetAnnotations()
```

### Nilai Kembali

Koleksi item anotasi; `null` jika ekstraksi anotasi tidak didukung.

### Lihat Juga

* class [AnnotationItem](../../../groupdocs.parser.data/annotationitem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetAnnotations(int) {#getannotations_1}

Mengekstrak anotasi dari halaman dokumen. Perhatikan bahwa hanya format PDF yang saat ini didukung.

```csharp
public IEnumerable<AnnotationItem> GetAnnotations(int pageIndex)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| pageIndex | Int32 | Indeks halaman berbasis nol. |

### Nilai Kembali

Koleksi item anotasi; `null` jika ekstraksi anotasi tidak didukung.

### Lihat Juga

* class [AnnotationItem](../../../groupdocs.parser.data/annotationitem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
