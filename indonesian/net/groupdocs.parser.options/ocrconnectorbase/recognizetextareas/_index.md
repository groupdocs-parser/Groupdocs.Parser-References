---
title: "RecognizeTextAreas"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mengenali area teks dari aliran imageStream."
type: docs
weight: 40
url: /id/net/groupdocs.parser.options/ocrconnectorbase/recognizetextareas/
---

## RecognizeTextAreas(Stream, Page, OcrOptions) {#recognizetextareas}

Mengenali area teks dari aliran *imageStream*.

```csharp
public virtual IList<PageTextArea> RecognizeTextAreas(Stream imageStream, Page page, 
    OcrOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| imageStream | Stream | Representasi gambar dari halaman dokumen. |
| page | Page | Halaman dokumen. |
| options | OcrOptions | Opsi OCR. |

### Nilai Kembali

Koleksi objek [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea); `null` jika pengenalan area teks tidak didukung.

### Lihat Juga

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Page](../../../groupdocs.parser.data/page)
* class [OcrOptions](../../ocroptions)
* class [OcrConnectorBase](../../ocrconnectorbase)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## RecognizeTextAreas(Stream, IEnumerable&lt;Rectangle&gt;, string, Page, OcrOptions) {#recognizetextareas_3}

Mengenali area teks dari aliran *imageStream*.

```csharp
public virtual IList<PageTextArea> RecognizeTextAreas(Stream imageStream, 
    IEnumerable<Rectangle> rectangles, string allowedSymbols, Page page, OcrOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| imageStream | Stream | Representasi gambar dari halaman dokumen. |
| rectangles | IEnumerable`1 | Koleksi area persegi panjang yang membatasi fungsionalitas OCR. |
| allowedSymbols | String | Filter simbol yang diizinkan oleh OCR. |
| page | Page | Halaman dokumen. |
| options | OcrOptions | Opsi OCR. |

### Nilai Kembali

Koleksi objek [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea); `null` jika pengenalan area teks tidak didukung.

### Lihat Juga

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Rectangle](../../../groupdocs.parser.data/rectangle)
* class [Page](../../../groupdocs.parser.data/page)
* class [OcrOptions](../../ocroptions)
* class [OcrConnectorBase](../../ocrconnectorbase)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
