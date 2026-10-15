---
title: "SetLicense"
second_title: "GroupDocs.Parser für .NET API-Referenz"
description: "Lizenziert die Komponente."
type: docs
weight: 20
url: /de/net/groupdocs.parser/license/setlicense/
---

## SetLicense(string) {#setlicense_1}

Lizenziert die Komponente.

```csharp
public void SetLicense(string filePath)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| filePath | String | Absoluter Pfad zur Lizenzdatei. |

### Beispiele

Das folgende Beispiel demonstriert, wie eine Lizenz gesetzt wird, indem ein Pfad zur Lizenzdatei übergeben wird.

```csharp
string licensePath = "LicenseFile.lic"";
GroupDocs.Parser.License license = new GroupDocs.Parser.License();
lic.SetLicense(licensePath);
```

### Siehe auch

* class [License](../../license)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## SetLicense(Stream) {#setlicense}

Lizenziert die Komponente.

```csharp
public void SetLicense(Stream stream)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | Stream | Lizenz‑Stream. |

### Beispiele

Das folgende Beispiel demonstriert, wie eine Lizenz gesetzt wird, indem ein Stream der Lizenzdatei übergeben wird.

```csharp
using (FileStream licenseStream = new FileStream("LicenseFile.lic", FileMode.Open))
{
    GroupDocs.Parser.License license = new GroupDocs.Parser.License();
    license.SetLicense(licenseStream);
}
```

### Siehe auch

* class [License](../../license)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NICHT BEARBEITEN: erstellt von xmldocmd für GroupDocs.Parser.dll -->
