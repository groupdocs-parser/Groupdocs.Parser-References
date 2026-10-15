---
title: "SetLicense"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "घटक को लाइसेंस करता है।"
type: docs
weight: 20
url: /hi/net/groupdocs.parser/license/setlicense/
---

## SetLicense(string) {#setlicense_1}

घटक को लाइसेंस करता है।

```csharp
public void SetLicense(string filePath)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | स्ट्रिंग | लाइसेंस फ़ाइल का पूर्ण पथ। |

### Examples

निम्न उदाहरण दिखाता है कि लाइसेंस सेट करने के लिए लाइसेंस फ़ाइल के पथ को कैसे पास किया जाए।

```csharp
string licensePath = "LicenseFile.lic"";
GroupDocs.Parser.License license = new GroupDocs.Parser.License();
lic.SetLicense(licensePath);
```

### संबंधित देखें

* class [License](../../license)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## SetLicense(Stream) {#setlicense}

घटक को लाइसेंस करता है।

```csharp
public void SetLicense(Stream stream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | Stream | लाइसेंस स्ट्रीम। |

### Examples

निम्न उदाहरण दिखाता है कि लाइसेंस सेट करने के लिए लाइसेंस फ़ाइल की स्ट्रीम को कैसे पास किया जाए।

```csharp
using (FileStream licenseStream = new FileStream("LicenseFile.lic", FileMode.Open))
{
    GroupDocs.Parser.License license = new GroupDocs.Parser.License();
    license.SetLicense(licenseStream);
}
```

### संबंधित देखें

* class [License](../../license)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
