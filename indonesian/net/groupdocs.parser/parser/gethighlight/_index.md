---
title: "GetHighlight"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mengekstrak sorotan dari dokumen."
type: docs
weight: 110
url: /id/net/groupdocs.parser/parser/gethighlight/
---

## Parser.GetHighlight method

Mengekstrak sorotan dari dokumen.

```csharp
public HighlightItem GetHighlight(int position, bool isDirect, HighlightOptions options)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| posisi | Int32 | Posisi awal sorotan. |
| isDirect | Boolean | Nilai yang menunjukkan apakah ekstraksi sorotan bersifat langsung. `true` jika sorotan diekstrak di sebelah kanan *position*; selain itu, `false`. |
| options | HighlightOptions | Opsi ekstraksi sorotan. |

### Nilai Kembali

Sebuah instance dari kelas [`HighlightItem`](../../../groupdocs.parser.data/highlightitem) yang mewakili sorotan yang diekstrak; `null` jika ekstraksi sorotan tidak didukung.

### Catatan

**Learn more:**

* [Extract highlights](https://docs.groupdocs.com/display/parsernet/Extract+highlights)

### Contoh

Contoh berikut menunjukkan cara mengekstrak sorotan yang berisi 3 kata:

```csharp
// Buat sebuah instance dari kelas Parser
using (Parser parser = new Parser(filePath))
{
    // Ekstrak sorotan:
    HighlightItem hl = parser.GetHighlight(2, true, new HighlightOptions(3));
    
    // Periksa apakah ekstraksi sorotan didukung
    if (hl == null)
    {
        Console.WriteLine("Highlight extraction isn't supported");
        return;
    }
    
    // Cetak sorotan yang diekstrak
    Console.WriteLine(string.Format("At {0}: {1}", hl.Position, hl.Text));
}
```

### Lihat Juga

* class [HighlightItem](../../../groupdocs.parser.data/highlightitem)
* class [HighlightOptions](../../../groupdocs.parser.options/highlightoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
