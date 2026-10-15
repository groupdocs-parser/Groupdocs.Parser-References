---
title: "OcrEventHandler"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "OCR इवेंट्स के लिए एक हैंडलर प्रदान करता है।"
type: docs
weight: 440
url: /hi/net/groupdocs.parser.options/ocreventhandler/
---

## OcrEventHandler class

OCR इवेंट्स के लिए एक हैंडलर प्रदान करता है।

```csharp
public class OcrEventHandler
```

## कंस्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [OcrEventHandler](ocreventhandler)() | एक नया उदाहरण प्रारंभ करता है [`OcrEventHandler`](../ocreventhandler) वर्ग का। |

## गुण

| नाम | विवरण |
| --- | --- |
| [HasWarnings](../../groupdocs.parser.options/ocreventhandler/haswarnings) { get; } | सूची में चेतावनियों के खाली न होने को दर्शाने वाला मान प्राप्त करता है। |
| [Warnings](../../groupdocs.parser.options/ocreventhandler/warnings) { get; } | चेतावनी संदेशों की सूची प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [GetWarnings](../../groupdocs.parser.options/ocreventhandler/getwarnings)(int) | *pageIndex* पृष्ठ के लिए चेतावनी संदेशों की सूची लौटाता है। |
| virtual [OnWarnings](../../groupdocs.parser.options/ocreventhandler/onwarnings)(int, IList&lt;string&gt;) | पृष्ठ के लिए चेतावनी संदेश सेट करता है। |

### संबंधित देखें

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
