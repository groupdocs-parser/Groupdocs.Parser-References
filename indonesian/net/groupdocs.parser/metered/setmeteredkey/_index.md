---
title: "SetMeteredKey"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Mengaktifkan produk dengan kunci Metered."
type: docs
weight: 20
url: /id/net/groupdocs.parser/metered/setmeteredkey/
---

## Metered.SetMeteredKey method

Mengaktifkan produk dengan kunci Metered.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| publicKey | String | Sebuah kunci publik. |
| privateKey | String | Sebuah kunci pribadi |

### Contoh

Contoh berikut menunjukkan cara mengaktifkan produk dengan kunci Metered.

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);
```

### Lihat Juga

* class [Metered](../../metered)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
