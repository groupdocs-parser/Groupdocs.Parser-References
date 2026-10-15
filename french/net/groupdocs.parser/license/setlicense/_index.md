---
title: "SetLicense"
second_title: "Référence API de GroupDocs.Parser pour .NET"
description: "Licence le composant."
type: docs
weight: 20
url: /fr/net/groupdocs.parser/license/setlicense/
---

## SetLicense(string) {#setlicense_1}

Licence le composant.

```csharp
public void SetLicense(string filePath)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | Chaîne | Chemin absolu vers le fichier de licence. |

### Exemples

L'exemple suivant montre comment définir une licence en passant un chemin vers le fichier de licence.

```csharp
string licensePath = "LicenseFile.lic"";
GroupDocs.Parser.License license = new GroupDocs.Parser.License();
lic.SetLicense(licensePath);
```

### Voir aussi

* class [License](../../license)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## SetLicense(Stream) {#setlicense}

Licence le composant.

```csharp
public void SetLicense(Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| flux | Stream | Flux de licence. |

### Exemples

L'exemple suivant montre comment définir une licence en passant le flux du fichier de licence.

```csharp
using (FileStream licenseStream = new FileStream("LicenseFile.lic", FileMode.Open))
{
    GroupDocs.Parser.License license = new GroupDocs.Parser.License();
    license.SetLicense(licenseStream);
}
```

### Voir aussi

* class [License](../../license)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour GroupDocs.Parser.dll -->
