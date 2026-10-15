---
title: "FromExtension"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "फ़ाइल एक्सटेंशन को फ़ाइल प्रकार से मैप करता है।"
type: docs
weight: 930
url: /hi/net/groupdocs.parser.options/filetype/fromextension/
---

## FileType.FromExtension method

फ़ाइल एक्सटेंशन को फ़ाइल प्रकार से मैप करता है।

```csharp
public static FileType FromExtension(string extension)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| एक्सटेंशन | स्ट्रिंग | फ़ाइल एक्सटेंशन (बिंदु \".\" सहित)। |

### रिटर्न वैल्यू

जब फ़ाइल प्रकार समर्थित हो तो इसे वापस देता है, अन्यथा डिफ़ॉल्ट [`Unknown`](../unknown) फ़ाइल प्रकार वापस देता है।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentException | जब *extension* null या खाली स्ट्रिंग हो तो फेंका जाता है। |

### संबंधित देखें

* class [FileType](../../filetype)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
