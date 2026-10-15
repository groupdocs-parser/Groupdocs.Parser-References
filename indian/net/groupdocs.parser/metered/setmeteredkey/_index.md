---
title: "SetMeteredKey"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "Metered कुंजियों के साथ उत्पाद को सक्रिय करता है।"
type: docs
weight: 20
url: /hi/net/groupdocs.parser/metered/setmeteredkey/
---

## Metered.SetMeteredKey method

Metered कुंजियों के साथ उत्पाद को सक्रिय करता है।

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| publicKey | स्ट्रिंग | एक सार्वजनिक कुंजी। |
| privateKey | स्ट्रिंग | एक निजी कुंजी |

### Examples

निम्न उदाहरण दिखाता है कि मीटरड कुंजियों के साथ उत्पाद को कैसे सक्रिय किया जाए।

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);
```

### संबंधित देखें

* class [Metered](../../metered)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
