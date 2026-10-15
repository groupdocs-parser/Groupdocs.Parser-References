---
title: "Metadata"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mendapatkan koleksi item metadata."
type: docs
weight: 30
url: /id/net/groupdocs.parser.data/containeritem/metadata/
---

## ContainerItem.Metadata property

Mendapatkan koleksi item metadata.

```csharp
public IEnumerable<MetadataItem> Metadata { get; }
```

### Property Value

Koleksi objek [`MetadataItem`](../../metadataitem); kosong jika metadata tidak disetel.

### Catatan

Metadata ini mengacu pada elemen kontainer itu sendiri, bukan dokumen. Tergantung pada jenis kontainer, metadata dapat berisi item berikut:

**Email Attachments**

**Name**

**Description**

**content-type**

Tipe MIME dari konten lampiran.

**ZIP Archives**

**Name**

**Description**

**date**

Waktu dan tanggal saat file yang ditunjuk oleh Zip Entry terakhir diubah.

**disposition**

Untuk mendeteksi apakah lampiran gambar bersifat inline, metadata 'disposition' digunakan. Jika ada, nilainya dapat 'inline' atau 'attachment'.

**Outlook Storage**

**Name**

**Description**

**date**

Waktu dan tanggal saat item Outlook Storage terakhir diubah.

**email-sender**

Nilai bidang "sender".

**email-to**

Nilai bidang "to".

**subject**

Nilai bidang "subject".

### Lihat Juga

* class [MetadataItem](../../metadataitem)
* class [ContainerItem](../../containeritem)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
