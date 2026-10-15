---
title: "ट्रायपार्स"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "किनारों के स्ट्रिंग प्रतिनिधित्व को उसकी क्लास समकक्ष में परिवर्तित करता है। रिटर्न वैल्यू यह दर्शाता है कि परिवर्तन सफल हुआ या विफल।"
type: docs
weight: 90
url: /hi/net/groupdocs.parser.templates/templatelinkedpositionedges/tryparse/
---

## TemplateLinkedPositionEdges.TryParse method

किनारों के स्ट्रिंग प्रतिनिधित्व को उसकी क्लास समकक्ष में परिवर्तित करता है। रिटर्न वैल्यू यह दर्शाता है कि परिवर्तन सफल हुआ या विफल।

```csharp
public static bool TryParse(string s, out TemplateLinkedPositionEdges edges)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| s | स्ट्रिंग | एक स्ट्रिंग जिसमें बदलने के लिए किनारे होते हैं। |
| edges | TemplateLinkedPositionEdges& | जब मेथड लौटता है, तो यह [`TemplateLinkedPositionEdges`](../../templatelinkedpositionedges) क्लास का वह उदाहरण रखता है जो *s* पैरामीटर में निर्दिष्ट मान के बराबर है, यदि रूपांतरण सफल हो; अन्यथा, `null`। |

### रिटर्न वैल्यू

`true` यदि *s* सफलतापूर्वक परिवर्तित हो गया; अन्यथा, `false`।

### संबंधित देखें

* class [TemplateLinkedPositionEdges](../../templatelinkedpositionedges)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
