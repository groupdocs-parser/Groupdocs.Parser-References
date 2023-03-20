---
title: GetHyperlinks
second_title: GroupDocs.Parser .NET API संदर्भ के लिए
description: दस्तवेज़ से हइपरलंक नकलत है
type: docs
weight: 100
url: /hi/net/groupdocs.parser/parser/gethyperlinks/
---
## GetHyperlinks() {#gethyperlinks}

दस्तावेज़ से हाइपरलिंक निकालता है।

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks()
```

### प्रतिलाभ की मात्रा

का संग्रह[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) ऑब्जेक्ट्स; `व्यर्थ` अगर हाइपरलिंक निष्कर्षण समर्थित नहीं है.

### उदाहरण

निम्न उदाहरण दिखाता है कि संपूर्ण दस्तावेज़ से सभी हाइपरलिंक कैसे निकालें:

```csharp
// पार्सर वर्ग का एक उदाहरण बनाएँ
using (Parser parser = new Parser(filePath))
{
    // जांचें कि क्या दस्तावेज़ हाइपरलिंक निष्कर्षण का समर्थन करता है
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // दस्तावेज़ से हाइपरलिंक निकालें
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks();
    // हाइपरलिंक्स पर पुनरावृति
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // हाइपरलिंक टेक्स्ट प्रिंट करें
        Console.WriteLine(h.Text);
        // हाइपरलिंक यूआरएल प्रिंट करें
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### यह सभी देखें

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int) {#gethyperlinks_2}

दस्तावेज़ पृष्ठ से हाइपरलिंक निकालता है.

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageIndex | Int32 | शून्य-आधारित पृष्ठ अनुक्रमणिका। |

### प्रतिलाभ की मात्रा

का संग्रह[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) ऑब्जेक्ट्स; `व्यर्थ` अगर हाइपरलिंक निष्कर्षण समर्थित नहीं है.

### उदाहरण

निम्न उदाहरण दिखाता है कि दस्तावेज़ पृष्ठ से हाइपरलिंक कैसे निकालें:

```csharp
// पार्सर वर्ग का एक उदाहरण बनाएँ
using (Parser parser = new Parser(filePath))
{
    // जांचें कि क्या दस्तावेज़ हाइपरलिंक निष्कर्षण का समर्थन करता है
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // दस्तावेज़ की जानकारी प्राप्त करें
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // जांचें कि क्या दस्तावेज़ में पृष्ठ हैं
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    // पृष्ठों पर पुनरावृति
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // पेज नंबर प्रिंट करें 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // दस्तावेज़ पृष्ठ से हाइपरलिंक निकालें
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex);
        // हाइपरलिंक्स पर पुनरावृति
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // हाइपरलिंक टेक्स्ट प्रिंट करें
            Console.WriteLine(h.Text);
            // हाइपरलिंक यूआरएल प्रिंट करें
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
    }
}
```

### यह सभी देखें

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

---

## GetHyperlinks(PageAreaOptions) {#gethyperlinks_1}

अनुकूलन विकल्पों का उपयोग करके दस्तावेज़ से हाइपरलिंक निकालता है (हाइपरलिंक वाले आयताकार क्षेत्र को सेट करने के लिए)

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(PageAreaOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| options | PageAreaOptions | हाइपरलिंक निष्कर्षण के लिए विकल्प। |

### प्रतिलाभ की मात्रा

का संग्रह[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) ऑब्जेक्ट्स; `व्यर्थ` अगर हाइपरलिंक निष्कर्षण समर्थित नहीं है.

### उदाहरण

निम्न उदाहरण दिखाता है कि दस्तावेज़ पृष्ठ क्षेत्र से हाइपरलिंक कैसे निकालें:

```csharp
// पार्सर वर्ग का एक उदाहरण बनाएँ
using (Parser parser = new Parser(filePath))
{
    // जांचें कि क्या दस्तावेज़ हाइपरलिंक निष्कर्षण का समर्थन करता है
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // वे विकल्प बनाएं जो हाइपरलिंक निष्कर्षण के लिए उपयोग किए जाते हैं
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // दस्तावेज़ पृष्ठ क्षेत्र से हाइपरलिंक निकालें
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(options);
    // हाइपरलिंक्स पर पुनरावृति
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // हाइपरलिंक टेक्स्ट प्रिंट करें
        Console.WriteLine(h.Text);
        // हाइपरलिंक यूआरएल प्रिंट करें
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### यह सभी देखें

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int, PageAreaOptions) {#gethyperlinks_3}

अनुकूलन विकल्पों का उपयोग करके दस्तावेज़ पृष्ठ से हाइपरलिंक निकालता है (हाइपरलिंक वाले आयताकार क्षेत्र को सेट करने के लिए)

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex, PageAreaOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageIndex | Int32 | शून्य-आधारित पृष्ठ अनुक्रमणिका। |
| options | PageAreaOptions | हाइपरलिंक निष्कर्षण के लिए विकल्प। |

### प्रतिलाभ की मात्रा

का संग्रह[`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) ऑब्जेक्ट्स; `व्यर्थ` अगर हाइपरलिंक निष्कर्षण समर्थित नहीं है.

### उदाहरण

निम्न उदाहरण दिखाता है कि अनुकूलन विकल्पों का उपयोग करके दस्तावेज़ पृष्ठ क्षेत्र से हाइपरलिंक कैसे निकालें:

```csharp
// पार्सर वर्ग का एक उदाहरण बनाएँ
using (Parser parser = new Parser(filePath))
{
    // जांचें कि क्या दस्तावेज़ हाइपरलिंक निष्कर्षण का समर्थन करता है
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    
    // दस्तावेज़ की जानकारी प्राप्त करें
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // जांचें कि क्या दस्तावेज़ में पृष्ठ हैं
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // वे विकल्प बनाएं जो हाइपरलिंक निष्कर्षण के लिए उपयोग किए जाते हैं
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // पृष्ठों पर पुनरावृति
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // पेज नंबर प्रिंट करें 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));         
        // दस्तावेज़ पृष्ठ क्षेत्र से हाइपरलिंक निकालें
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex, options);
        // हाइपरलिंक्स पर पुनरावृति
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // हाइपरलिंक टेक्स्ट प्रिंट करें
            Console.WriteLine(h.Text);
            // हाइपरलिंक यूआरएल प्रिंट करें
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
}
```

### यह सभी देखें

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
