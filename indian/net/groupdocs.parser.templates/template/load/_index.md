---
title: "Load"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "फ़ाइल से टेम्पलेट लोड करता है।"
type: docs
weight: 20
url: /hi/net/groupdocs.parser.templates/template/load/
---

## Load(string) {#load_1}

फ़ाइल से टेम्पलेट लोड करता है।

```csharp
public static Template Load(string filePath)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | स्ट्रिंग | फ़ाइल का पथ। |

### रिटर्न वैल्यू

लोडेड टेम्प्लेट के साथ एक उदाहरण [`Template`](../../template) क्लास का।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| [GroupDocsParserException](../../../groupdocs.parser.exceptions/groupdocsparserexception) | फ़ाइल वैध फ़ॉर्मेट में टेम्प्लेट का प्रतिनिधित्व नहीं करती है। |

### संबंधित देखें

* class [Template](../../template)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

---

## Load(Stream) {#load}

स्ट्रीम से टेम्पलेट लोड करता है।

```csharp
public static Template Load(Stream stream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| स्ट्रीम | Stream | इनपुट स्ट्रीम। |

### रिटर्न वैल्यू

लोडेड टेम्प्लेट के साथ एक उदाहरण [`Template`](../../template) क्लास का।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| [GroupDocsParserException](../../../groupdocs.parser.exceptions/groupdocsparserexception) | स्ट्रीम वैध फ़ॉर्मेट में टेम्प्लेट का प्रतिनिधित्व नहीं करती है। |

### संबंधित देखें

* class [Template](../../template)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
