---
title: "WorksheetInfo"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Menginisialisasi instance baru dari kelas WorksheetInfogroupdocs.parser.data/worksheetinfo."
type: docs
weight: 10
url: /id/net/groupdocs.parser.data/worksheetinfo/worksheetinfo/
---

## WorksheetInfo constructor

Menginisialisasi instance baru dari kelas [`WorksheetInfo`](../../worksheetinfo).

```csharp
public WorksheetInfo(int index, string name, WorksheetRange range)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| indeks | Int32 | Indeks berbasis nol dari lembar kerja. |
| nama | String | Nilai string yang mewakili nama lembar kerja. |
| range | WorksheetRange | Instance dari kelas [`WorksheetRange`](../../worksheetrange) yang mewakili ukuran lembar kerja. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | Indeks lembar kerja tidak boleh negatif. |
| ArgumentNullException | Ukuran lembar kerja tidak boleh `null`. |

### Lihat Juga

* class [WorksheetRange](../../worksheetrange)
* class [WorksheetInfo](../../worksheetinfo)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
