---
title: "MoveTo"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "बिंदु में समान आकार के विभाजकों और स्थिति के साथ एक नया लेआउट बनाता है।"
type: docs
weight: 50
url: /hi/net/groupdocs.parser.templates/templatetablelayout/moveto/
---

## TemplateTableLayout.MoveTo method

एक नया लेआउट बनाता है जिसमें समान आकार, विभाजक और *पॉइंट* में स्थिति होती है।

```csharp
public TemplateTableLayout MoveTo(Point point)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| point | Point | नए लेआउट की स्थिति। |

### रिटर्न वैल्यू

*point* में समान आकार, विभाजक और स्थिति के साथ एक नया लेआउट।

### Examples

यह कार्यक्षमता Table Layout को स्थानांतरित करने की अनुमति देती है।

उदाहरण के लिए, एक दस्तावेज़ के प्रत्येक पृष्ठ पर तालिकाएँ होती हैं (या ऐसे दस्तावेज़ों का सेट जिसमें पृष्ठ पर एक तालिका होती है)। ये तालिकाएँ स्थिति और सामग्री में भिन्न होती हैं, लेकिन उनके कॉलम और पंक्तियाँ समान होती हैं। इस स्थिति में उपयोगकर्ता एक बार `(0, 0)` पर [`TemplateTableLayout`](../../templatetablelayout) ऑब्जेक्ट को परिभाषित कर सकता है और फिर इसे निश्चित तालिका के स्थान पर ले जा सकता है।

यदि तालिका की स्थिति पृष्ठ के अन्य ऑब्जेक्ट पर निर्भर करती है, तो उपयोगकर्ता टेम्पलेट दस्तावेज़ के आधार पर [`TemplateTableLayout`](../../templatetablelayout) ऑब्जेक्ट को परिभाषित कर सकता है और फिर इसे एंकर ऑब्जेक्ट के अनुसार ले जा सकता है। उदाहरण के लिए, यदि यह एक सारांश तालिका है और इसके बाद विवरण तालिका आती है (जिसमें पंक्तियों की संख्या अलग हो सकती है)। इस स्थिति में उपयोगकर्ता टेम्पलेट दस्तावेज़ पर (ज्ञात विवरण तालिका आयत के साथ) [`TemplateTableLayout`](../../templatetablelayout) ऑब्जेक्ट को परिभाषित कर सकता है और फिर टेम्पलेट और वास्तविक दस्तावेज़ की विवरण तालिका आयत के अंतर के अनुसार [`TemplateTableLayout`](../../templatetablelayout) ऑब्जेक्ट को ले जा सकता है।

`MoveTo` मेथड वर्तमान ऑब्जेक्ट की एक कॉपी लौटाता है। उपयोगकर्ता कोई भी निर्देशांक पास कर सकता है (यहाँ तक कि नकारात्मक - तब लेआउट बाएँ/ऊपर की ओर स्थानांतरित हो जाएगा)।

```csharp
// एक तालिका लेआउट बनाएं
TemplateTableLayout layout = new TemplateTableLayout(
    new double[] { 0, 25, 150, 180, 230 },
    new double[] { 0, 15, 30, 45, 60, 75 });

// एक आयत प्रिंट करें
Rectangle rect = layout.Rectangle;

// प्रिंट करता है: pos: (0, 0) size: (230, 75)
Console.WriteLine(string.Format("pos: ({0}, {1}) size: ({2}, {3})", rect.Left, rect.Top, rect.Size.Width, rect.Size.Height));

// लेआउट को निश्चित तालिका स्थान पर ले जाएँ
TemplateTableLayout movedLayout = layout.MoveTo(new Point(315, 250));

// सुनिश्चित करें कि पहले विभाजक स्थानांतरित हो गए हैं:
Console.WriteLine(movedLayout.VerticalSeparators[0]); // prints: 315
Console.WriteLine(movedLayout.HorizontalSeparators[0]); // prints: 250

Rectangle movedRect = movedLayout.Rectangle;

// प्रिंट करता है: pos: (315, 250) size: (230, 75)
Console.WriteLine(string.Format("pos: ({0}, {1}) size: ({2}, {3})", movedRect.Left, movedRect.Top, movedRect.Size.Width, movedRect.Size.Height));

// movedLayout ऑब्जेक्ट लेआउट ऑब्जेक्ट की एक कॉपी है, इसलिए हम मूल लेआउट पर प्रभाव डाले बिना विभाजकों को समायोजित कर सकते हैं:
movedLayout.HorizontalSeparators.Add(90);

Console.WriteLine(movedLayout.HorizontalSeparators.Count); // prints: 7
Console.WriteLine(layout.HorizontalSeparators.Count); // prints: 6
```

### संबंधित देखें

* class [Point](../../../groupdocs.parser.data/point)
* class [TemplateTableLayout](../../templatetablelayout)
* namespace [GroupDocs.Parser.Templates](../../../groupdocs.parser.templates)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
