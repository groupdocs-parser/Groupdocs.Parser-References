---
title: "Muat"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Memuat templat dari file."
type: docs
weight: 20
url: /id/net/groupdocs.parser.templates/template/load/
---

## Load(string) {#load_1}

Memuat templat dari file.

```csharp
public static Template Load(string filePath)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| filePath | String | Jalur ke file. |

### Nilai Kembali

Instance dari kelas [`Template`](../../template) dengan templat yang dimuat.

### Exceptions

| exception | condition |
| --- | --- |
| [GroupDocsParserException](../../../groupdocs.parser.exceptions/groupdocsparserexception) | File tidak mewakili templat dalam format yang valid. |

### Lihat Juga

* class [Template](../../template)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## Load(Stream) {#load}

Memuat templat dari aliran.

```csharp
public static Template Load(Stream stream)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| stream | Stream | Aliran masukan. |

### Nilai Kembali

Instance dari kelas [`Template`](../../template) dengan templat yang dimuat.

### Exceptions

| exception | condition |
| --- | --- |
| [GroupDocsParserException](../../../groupdocs.parser.exceptions/groupdocsparserexception) | Aliran tidak mewakili templat dalam format yang valid. |

### Lihat Juga

* class [Template](../../template)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
