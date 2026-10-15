---
title: "GetHyperlinks"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "दस्तावेज़ से हाइपरलिंक निकालता है।"
type: docs
weight: 120
url: /hi/net/groupdocs.parser/parser/gethyperlinks/
---

## GetHyperlinks() {#gethyperlinks}

दस्तावेज़ से हाइपरलिंक निकालता है।

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks()
```

### रिटर्न वैल्यू

एक संग्रह [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) ऑब्जेक्ट्स का; यदि हाइपरलिंक निष्कर्षण समर्थित नहीं है तो `null`।

### Examples

निम्न उदाहरण दिखाता है कि पूरे दस्तावेज़ से सभी हाइपरलिंक कैसे निकाले जाएँ:

```csharp
// Parser class का एक instance बनाएं
using (Parser parser = new Parser(filePath))
{
    // जाँचें कि दस्तावेज़ हाइपरलिंक निष्कर्षण का समर्थन करता है या नहीं
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // दस्तावेज़ से हाइपरलिंक निकालें
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks();
    // हाइपरलिंक पर इटररेट करें
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // हाइपरलिंक टेक्स्ट प्रिंट करें
        Console.WriteLine(h.Text);
        // हाइपरलिंक URL प्रिंट करें
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### संबंधित देखें

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int) {#gethyperlinks_2}

दस्तावेज़ पृष्ठ से हाइपरलिंक निकालता है।

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageIndex | Int32 | शून्य-आधारित पेज इंडेक्स। |

### रिटर्न वैल्यू

एक संग्रह [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) ऑब्जेक्ट्स का; यदि हाइपरलिंक निष्कर्षण समर्थित नहीं है तो `null`।

### Examples

निम्न उदाहरण दिखाता है कि दस्तावेज़ पृष्ठ से हाइपरलिंक कैसे निकाले जाएँ:

```csharp
// Parser class का एक instance बनाएं
using (Parser parser = new Parser(filePath))
{
    // जाँचें कि दस्तावेज़ हाइपरलिंक निष्कर्षण का समर्थन करता है या नहीं
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // दस्तावेज़ की जानकारी प्राप्त करें
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // जाँचें कि दस्तावेज़ में पृष्ठ हैं या नहीं
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    // पृष्ठों पर इटररेट करें
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // पृष्ठ संख्या प्रिंट करें 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // दस्तावेज़ पृष्ठ से हाइपरलिंक निकालें
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex);
        // हाइपरलिंक पर इटररेट करें
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // हाइपरलिंक टेक्स्ट प्रिंट करें
            Console.WriteLine(h.Text);
            // हाइपरलिंक URL प्रिंट करें
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
    }
}
```

### संबंधित देखें

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(PageAreaOptions) {#gethyperlinks_1}

कस्टमाइज़ेशन विकल्पों का उपयोग करके दस्तावेज़ से हाइपरलिंक निकालता है (हाइपरलिंक वाले आयताकार क्षेत्र को सेट करने के लिए)।

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(PageAreaOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| options | PageAreaOptions | हाइपरलिंक निष्कर्षण के विकल्प। |

### रिटर्न वैल्यू

एक संग्रह [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) ऑब्जेक्ट्स का; यदि हाइपरलिंक निष्कर्षण समर्थित नहीं है तो `null`।

### Examples

निम्न उदाहरण दिखाता है कि दस्तावेज़ पृष्ठ क्षेत्र से हाइपरलिंक कैसे निकाले जाएँ:

```csharp
// Parser class का एक instance बनाएं
using (Parser parser = new Parser(filePath))
{
    // जाँचें कि दस्तावेज़ हाइपरलिंक निष्कर्षण का समर्थन करता है या नहीं
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    // हाइपरलिंक निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प बनाएं
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // दस्तावेज़ पृष्ठ क्षेत्र से हाइपरलिंक निकालें
    IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(options);
    // हाइपरलिंक पर इटररेट करें
    foreach (PageHyperlinkArea h in hyperlinks)
    {
        // हाइपरलिंक टेक्स्ट प्रिंट करें
        Console.WriteLine(h.Text);
        // हाइपरलिंक URL प्रिंट करें
        Console.WriteLine(h.Url);
        Console.WriteLine();
    }
}
```

### संबंधित देखें

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetHyperlinks(int, PageAreaOptions) {#gethyperlinks_3}

कस्टमाइज़ेशन विकल्पों का उपयोग करके दस्तावेज़ पृष्ठ से हाइपरलिंक निकालता है (हाइपरलिंक वाले आयताकार क्षेत्र को सेट करने के लिए)।

```csharp
public IEnumerable<PageHyperlinkArea> GetHyperlinks(int pageIndex, PageAreaOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageIndex | Int32 | शून्य-आधारित पेज इंडेक्स। |
| options | PageAreaOptions | हाइपरलिंक निष्कर्षण के विकल्प। |

### रिटर्न वैल्यू

एक संग्रह [`PageHyperlinkArea`](../../../groupdocs.parser.data/pagehyperlinkarea) ऑब्जेक्ट्स का; यदि हाइपरलिंक निष्कर्षण समर्थित नहीं है तो `null`।

### Examples

निम्न उदाहरण दिखाता है कि कैसे अनुकूलन विकल्पों का उपयोग करके दस्तावेज़ पृष्ठ क्षेत्र से हाइपरलिंक निकाले जाएँ:

```csharp
// Parser class का एक instance बनाएं
using (Parser parser = new Parser(filePath))
{
    // जाँचें कि दस्तावेज़ हाइपरलिंक निष्कर्षण का समर्थन करता है या नहीं
    if (!parser.Features.Hyperlinks)
    {
        Console.WriteLine("Document isn't supports hyperlink extraction.");
        return;
    }
    
    // दस्तावेज़ की जानकारी प्राप्त करें
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // जाँचें कि दस्तावेज़ में पृष्ठ हैं या नहीं
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    
    // हाइपरलिंक निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प बनाएं
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(380, 90), new Size(150, 50)));
    // पृष्ठों पर इटररेट करें
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // पृष्ठ संख्या प्रिंट करें 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));         
        // दस्तावेज़ पृष्ठ क्षेत्र से हाइपरलिंक निकालें
        IEnumerable<PageHyperlinkArea> hyperlinks = parser.GetHyperlinks(pageIndex, options);
        // हाइपरलिंक पर इटररेट करें
        foreach (PageHyperlinkArea h in hyperlinks)
        {
            // हाइपरलिंक टेक्स्ट प्रिंट करें
            Console.WriteLine(h.Text);
            // हाइपरलिंक URL प्रिंट करें
            Console.WriteLine(h.Url);
            Console.WriteLine();
        }
}
```

### संबंधित देखें

* class [PageHyperlinkArea](../../../groupdocs.parser.data/pagehyperlinkarea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
