---
title: "ReleasePageStream"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "एक मेथड को दर्शाता है जो CreatePageStream./createpagestream डेलीगेट द्वारा निर्मित स्ट्रीम को रिलीज़ करता है।"
type: docs
weight: 580
url: /hi/net/groupdocs.parser.options/releasepagestream/
---

## ReleasePageStream delegate

एक मेथड को दर्शाता है जो [`CreatePageStream`](../createpagestream) डेलीगेट द्वारा निर्मित स्ट्रीम को रिलीज़ करता है।

```csharp
public delegate void ReleasePageStream(int pageNumber, Stream pageStream);
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageNumber | Int32 | जेनरेट किए गए पेज प्रीव्यू का पेज नंबर। |
| pageStream | Stream | जेनरेट किए गए पेज प्रीव्यू को समाहित करने वाला स्ट्रीम। |

### संबंधित देखें

* namespace [GroupDocs.Parser.Options](../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
