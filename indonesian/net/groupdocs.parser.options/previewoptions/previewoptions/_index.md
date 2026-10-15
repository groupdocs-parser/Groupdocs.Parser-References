---
title: "PreviewOptions"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menginisialisasi instance baru dari kelas PreviewOptionsgroupdocs.parser.options/previewoptions yang menyebabkan aliran keluaran ditutup."
type: docs
weight: 10
url: /id/net/groupdocs.parser.options/previewoptions/previewoptions/
---

## PreviewOptions(CreatePageStream) {#constructor}

Menginisialisasi instance baru dari kelas [`PreviewOptions`](../../previewoptions) yang menyebabkan aliran keluaran ditutup.

```csharp
public PreviewOptions(CreatePageStream createPageStream)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| createPageStream | CreatePageStream | Membuat aliran untuk pratinjau halaman tertentu. |

### Lihat Juga

* delegate [CreatePageStream](../../createpagestream)
* class [PreviewOptions](../../previewoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PreviewOptions(CreatePageStream, ReleasePageStream) {#constructor_1}

Menginisialisasi instance baru dari kelas [`PreviewOptions`](../../previewoptions) yang menyebabkan aliran keluaran dikembalikan ke klien untuk penggunaan lebih lanjut.

```csharp
public PreviewOptions(CreatePageStream createPageStream, ReleasePageStream releasePageStream)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| createPageStream | CreatePageStream | Membuat aliran untuk pratinjau halaman tertentu |
| releasePageStream | ReleasePageStream | Memberitahukan bahwa pembuatan pratinjau halaman selesai dan mendapatkan aliran keluaran. |

### Lihat Juga

* delegate [CreatePageStream](../../createpagestream)
* delegate [ReleasePageStream](../../releasepagestream)
* class [PreviewOptions](../../previewoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
