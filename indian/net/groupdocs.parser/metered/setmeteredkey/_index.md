---
title: SetMeteredKey
second_title: GroupDocs.Parser .NET API संदर्भ के लिए
description: मटर्ड कुंजयं के सथ उत्पद क सक्रय करत है
type: docs
weight: 20
url: /hi/net/groupdocs.parser/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

मीटर्ड कुंजियों के साथ उत्पाद को सक्रिय करता है।

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| publicKey | String | एक सार्वजनिक कुंजी। |
| privateKey | String | एक निजी कुंजी |

### उदाहरण

निम्नलिखित उदाहरण प्रदर्शित करता है कि मीटर्ड कुंजियों के साथ उत्पाद को कैसे सक्रिय किया जाए।

```csharp
string publicKey = "Public Key";
string privateKey = "Private Key";

Metered metered = new Metered();
metered.SetMeteredKey(publicKey, privateKey);
```

### यह सभी देखें

* class [Metered](../../metered)
* नाम स्थान [GroupDocs.Parser](../../metered)
* सभा [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->