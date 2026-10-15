---
title: "TryParse"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mengonversi representasi string dari sebuah titik ke ekuivalen kelasnya. Nilai kembali menunjukkan apakah konversi berhasil atau gagal."
type: docs
weight: 80
url: /id/net/groupdocs.parser.data/point/tryparse/
---

## Point.TryParse method

Mengonversi representasi string dari sebuah titik ke ekuivalen kelasnya. Nilai kembali menunjukkan apakah konversi berhasil atau gagal.

```csharp
public static bool TryParse(string s, out Point point)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| s | String | String yang berisi sebuah titik untuk dikonversi. |
| point | Point& | Saat metode mengembalikan, ia berisi instance kelas [`Point`](../../point) yang setara dengan nilai yang ditentukan dalam parameter *s*, jika konversi berhasil; jika tidak, `null`. |

### Nilai Kembali

`true` jika *s* berhasil dikonversi; jika tidak, `false`.

### Lihat Juga

* class [Point](../../point)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
