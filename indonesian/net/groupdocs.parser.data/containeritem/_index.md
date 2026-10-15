---
title: "ContainerItem"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mewakili item kontainer seperti entitas arsip Zip, lampiran email, item PDF Portfolio, dan seterusnya."
type: docs
weight: 720
url: /id/net/groupdocs.parser.data/containeritem/
---

## ContainerItem class

Mewakili item kontainer seperti entitas arsip Zip, lampiran email, item PDF Portfolio, dan sebagainya.

```csharp
public sealed class ContainerItem
```

## Properti

| Nama | Deskripsi |
| --- | --- |
| [Directory](../../groupdocs.parser.data/containeritem/directory) { get; } | Mendapatkan direktori item. |
| [FilePath](../../groupdocs.parser.data/containeritem/filepath) { get; } | Mendapatkan jalur lengkap item. |
| [Metadata](../../groupdocs.parser.data/containeritem/metadata) { get; } | Mendapatkan koleksi item metadata. |
| [Name](../../groupdocs.parser.data/containeritem/name) { get; } | Mendapatkan nama item. |
| [Size](../../groupdocs.parser.data/containeritem/size) { get; } | Mendapatkan ukuran item. |

## Metode

| Nama | Deskripsi |
| --- | --- |
| [DetectFileType](../../groupdocs.parser.data/containeritem/detectfiletype)(FileTypeDetectionMode) | Mendeteksi tipe file dari item kontainer. |
| [GetMetadataValue](../../groupdocs.parser.data/containeritem/getmetadatavalue)(string) | Mendapatkan nilai metadata. |
| [OpenParser](../../groupdocs.parser.data/containeritem/openparser#openparser)() | Membuat objek [`Parser`](../../groupdocs.parser/parser) untuk konten item. |
| [OpenParser](../../groupdocs.parser.data/containeritem/openparser#openparser_1)(LoadOptions) | Membuat objek [`Parser`](../../groupdocs.parser/parser) untuk konten item dengan [`LoadOptions`](../../groupdocs.parser.options/loadoptions). |
| [OpenParser](../../groupdocs.parser.data/containeritem/openparser#openparser_2)(LoadOptions, ParserSettings) | Membuat objek [`Parser`](../../groupdocs.parser/parser) untuk konten item dengan [`LoadOptions`](../../groupdocs.parser.options/loadoptions) dan [`ParserSettings`](../../groupdocs.parser.options/parsersettings). |
| [OpenStream](../../groupdocs.parser.data/containeritem/openstream)() | Membuka aliran konten item. |

### Catatan

Sebuah instance kelas [`ContainerItem`](../containeritem) digunakan sebagai nilai kembali dari metode [`GetContainer`](../../groupdocs.parser/parser/getcontainer). Lihat contoh penggunaan di sana.

### Lihat Juga

* namespace [GroupDocs.Parser.Data](../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
