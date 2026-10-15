---
title: "PreviewOptions"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "एक नया उदाहरण प्रारंभ करता है PreviewOptionsgroupdocs.parser.options/previewoptions क्लास का जिससे आउटपुट स्ट्रीम बंद हो जाता है।"
type: docs
weight: 10
url: /hi/net/groupdocs.parser.options/previewoptions/previewoptions/
---

## PreviewOptions(CreatePageStream) {#constructor}

एक नया उदाहरण प्रारंभ करता है [`PreviewOptions`](../../previewoptions) क्लास का जिससे आउटपुट स्ट्रीम बंद हो जाता है।

```csharp
public PreviewOptions(CreatePageStream createPageStream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| createPageStream | CreatePageStream | एक विशिष्ट पृष्ठ प्रीव्यू के लिए स्ट्रीम बनाता है। |

### संबंधित देखें

* delegate [CreatePageStream](../../createpagestream)
* class [PreviewOptions](../../previewoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## PreviewOptions(CreatePageStream, ReleasePageStream) {#constructor_1}

एक नया उदाहरण प्रारंभ करता है [`PreviewOptions`](../../previewoptions) क्लास का जिससे आउटपुट स्ट्रीम क्लाइंट को आगे उपयोग के लिए वापस किया जाता है।

```csharp
public PreviewOptions(CreatePageStream createPageStream, ReleasePageStream releasePageStream)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| createPageStream | CreatePageStream | एक विशिष्ट पृष्ठ प्रीव्यू के लिए स्ट्रीम बनाता है |
| releasePageStream | ReleasePageStream | सूचित करता है कि पृष्ठ प्रीव्यू निर्माण समाप्त हो गया है और आउटपुट स्ट्रीम प्राप्त करता है। |

### संबंधित देखें

* delegate [CreatePageStream](../../createpagestream)
* delegate [ReleasePageStream](../../releasepagestream)
* class [PreviewOptions](../../previewoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
