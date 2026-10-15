---
title: "RecognizeText"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mengenali teks dari stream imageStream."
type: docs
weight: 30
url: /id/net/groupdocs.parser.options/ocrconnectorbase/recognizetext/
---

## OcrConnectorBase.RecognizeText method

Mengenali teks dari aliran *imageStream*.

```csharp
public virtual string RecognizeText(Stream imageStream, OcrOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| imageStream | Stream | Representasi gambar dari halaman dokumen. |
| options | OcrOptions | Opsi OCR. |

### Nilai Kembali

String yang mewakili teks yang dikenali; `null` jika pengenalan teks tidak didukung.

### Lihat Juga

* class [OcrOptions](../../ocroptions)
* class [OcrConnectorBase](../../ocrconnectorbase)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
