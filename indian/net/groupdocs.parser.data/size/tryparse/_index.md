---
title: "ट्रायपार्स"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "आकार की स्ट्रिंग प्रतिनिधित्व को उसकी क्लास समकक्ष में परिवर्तित करता है। रिटर्न मान यह दर्शाता है कि परिवर्तन सफल हुआ या विफल।"
type: docs
weight: 70
url: /hi/net/groupdocs.parser.data/size/tryparse/
---

## Size.TryParse method

आकार की स्ट्रिंग प्रतिनिधित्व को उसकी क्लास समकक्ष में परिवर्तित करता है। रिटर्न मान यह दर्शाता है कि परिवर्तन सफल हुआ या विफल।

```csharp
public static bool TryParse(string s, out Size size)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| s | स्ट्रिंग | एक स्ट्रिंग जिसमें परिवर्तित करने के लिए आकार होता है। |
| size | Size& | जब मेथड रिटर्न करता है, तो यह [`Size`](../../size) क्लास का इंस्टेंस रखता है जो *s* पैरामीटर में निर्दिष्ट मान के बराबर है, यदि रूपांतरण सफल हुआ; अन्यथा, `null`। |

### रिटर्न वैल्यू

`true` यदि *s* सफलतापूर्वक परिवर्तित हो गया; अन्यथा, `false`।

### संबंधित देखें

* class [Size](../../size)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
