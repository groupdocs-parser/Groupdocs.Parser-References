---
title: "SetLicense"
second_title: "Referensi API GroupDocs.Parser untuk .NET"
description: "Memberi lisensi komponen."
type: docs
weight: 20
url: /id/net/groupdocs.parser/license/setlicense/
---

## SetLicense(string) {#setlicense_1}

Memberi lisensi komponen.

```csharp
public void SetLicense(string filePath)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| filePath | String | Jalur absolut ke file lisensi. |

### Contoh

Contoh berikut menunjukkan cara mengatur lisensi dengan memberikan jalur ke file lisensi.

```csharp
string licensePath = "LicenseFile.lic"";
GroupDocs.Parser.License license = new GroupDocs.Parser.License();
lic.SetLicense(licensePath);
```

### Lihat Juga

* class [License](../../license)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## SetLicense(Stream) {#setlicense}

Memberi lisensi komponen.

```csharp
public void SetLicense(Stream stream)
```

| Parameter | Type | Deskripsi |
| --- | --- | --- |
| stream | Stream | Aliran lisensi. |

### Contoh

Contoh berikut menunjukkan cara mengatur lisensi dengan memberikan Stream dari file lisensi.

```csharp
using (FileStream licenseStream = new FileStream("LicenseFile.lic", FileMode.Open))
{
    GroupDocs.Parser.License license = new GroupDocs.Parser.License();
    license.SetLicense(licenseStream);
}
```

### Lihat Juga

* class [License](../../license)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- JANGAN EDIT: dihasilkan oleh xmldocmd untuk GroupDocs.Parser.dll -->
