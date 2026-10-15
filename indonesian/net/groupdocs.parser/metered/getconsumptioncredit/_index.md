---
title: "GetConsumptionCredit"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mengambil jumlah kredit yang digunakan."
type: docs
weight: 30
url: /id/net/groupdocs.parser/metered/getconsumptioncredit/
---

## Metered.GetConsumptionCredit method

Mengambil jumlah kredit yang digunakan.

```csharp
public static decimal GetConsumptionCredit()
```

### Nilai Kembali

Nilai desimal yang mewakili kredit konsumsi.

### Contoh

Contoh berikut menunjukkan cara mengambil jumlah kredit yang dikonsumsi.

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);

decimal creditsConsumed = Metered.GetConsumptionCredit();
```

### Lihat Juga

* class [Metered](../../metered)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
