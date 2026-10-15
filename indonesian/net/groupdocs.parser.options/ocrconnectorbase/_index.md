---
title: "OcrConnectorBase"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menyediakan fungsionalitas OCR."
type: docs
weight: 430
url: /id/net/groupdocs.parser.options/ocrconnectorbase/
---

## OcrConnectorBase class

Menyediakan fungsionalitas OCR.

```csharp
public abstract class OcrConnectorBase
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| virtual [IsTextAreasSupported](../../groupdocs.parser.options/ocrconnectorbase/istextareassupported) { get; } | Mendapatkan nilai yang menunjukkan apakah ekstraksi area teks didukung. |
| virtual [IsTextSupported](../../groupdocs.parser.options/ocrconnectorbase/istextsupported) { get; } | Mendapatkan nilai yang menunjukkan apakah ekstraksi teks didukung. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| virtual [RecognizeText](../../groupdocs.parser.options/ocrconnectorbase/recognizetext#recognizetext)(Stream, OcrOptions) | Mengenali teks dari aliran *imageStream*. |
| virtual [RecognizeTextAreas](../../groupdocs.parser.options/ocrconnectorbase/recognizetextareas#recognizetextareas)(Stream, Page, OcrOptions) | Mengenali area teks dari aliran *imageStream*. |
| virtual [RecognizeTextAreas](../../groupdocs.parser.options/ocrconnectorbase/recognizetextareas#recognizetextareas_3)(Stream, IEnumerable&lt;Rectangle&gt;, string, Page, OcrOptions) | Mengenali area teks dari aliran *imageStream*. |

### Lihat Juga

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
