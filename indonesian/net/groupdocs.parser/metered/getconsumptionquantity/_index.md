---
title: "GetConsumptionQuantity"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mengambil jumlah MB yang diproses."
type: docs
weight: 40
url: /id/net/groupdocs.parser/metered/getconsumptionquantity/
---

## Metered.GetConsumptionQuantity method

Mengambil jumlah MB yang diproses.

```csharp
public static decimal GetConsumptionQuantity()
```

### Nilai Kembali

Nilai desimal yang mewakili kuantitas konsumsi.

### Contoh

Contoh berikut menunjukkan cara mengambil jumlah MB yang diproses.

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);

decimal mbProcessed = Metered.GetConsumptionQuantity();
```

### Lihat Juga

* class [Metered](../../metered)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
