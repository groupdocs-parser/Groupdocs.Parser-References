---
title: "ट्रायपार्स"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "एक बिंदु की स्ट्रिंग प्रतिनिधित्व को उसके क्लास समकक्ष में परिवर्तित करता है। एक रिटर्न वैल्यू संकेत देता है कि रूपांतरण सफल हुआ या विफल।"
type: docs
weight: 80
url: /hi/net/groupdocs.parser.data/point/tryparse/
---

## Point.TryParse method

एक बिंदु की स्ट्रिंग प्रतिनिधित्व को उसके क्लास समकक्ष में परिवर्तित करता है। एक रिटर्न वैल्यू संकेत देता है कि रूपांतरण सफल हुआ या विफल।

```csharp
public static bool TryParse(string s, out Point point)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| s | स्ट्रिंग | एक स्ट्रिंग जिसमें परिवर्तित करने के लिए बिंदु शामिल है। |
| point | Point& | जब मेथड लौटता है, तो यह [`Point`](../../point) क्लास का वह उदाहरण रखता है जो *s* पैरामीटर में निर्दिष्ट मान के बराबर है, यदि रूपांतरण सफल हुआ; अन्यथा, `null`। |

### रिटर्न वैल्यू

`true` यदि *s* सफलतापूर्वक परिवर्तित हो गया; अन्यथा, `false`।

### संबंधित देखें

* class [Point](../../point)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
