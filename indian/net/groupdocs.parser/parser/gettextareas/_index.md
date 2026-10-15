---
title: "GetTextAreas"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "दस्तावेज़ से पाठ क्षेत्रों को निकालता है।"
type: docs
weight: 190
url: /hi/net/groupdocs.parser/parser/gettextareas/
---

## GetTextAreas() {#gettextareas}

दस्तावेज़ से पाठ क्षेत्रों को निकालता है।

```csharp
public IEnumerable<PageTextArea> GetTextAreas()
```

### रिटर्न वैल्यू

एक संग्रह [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) वस्तुओं का; यदि टेक्स्ट एरिया निष्कर्षण समर्थित नहीं है तो `null`।

### टिप्पणियाँ

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Examples

निम्नलिखित उदाहरण दिखाता है कि पूरे दस्तावेज़ से सभी टेक्स्ट एरिया कैसे निकालें:

```csharp
// Parser class का एक instance बनाएं
using(Parser parser = new Parser(filePath))
{
    // टेक्स्ट एरिया निकालें
    IEnumerable<PageTextArea> areas = parser.GetTextAreas();
    // जाँचें कि टेक्स्ट एरिया निष्कर्षण समर्थित है या नहीं
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // पृष्ठ टेक्स्ट एरिया पर पुनरावृति करें
    foreach(PageTextArea a in areas)
    {
        // एक पृष्ठ अनुक्रमांक, आयत और टेक्स्ट एरिया मान को प्रिंट करें:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### संबंधित देखें

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(PageTextAreaOptions) {#gettextareas_1}

दस्तावेज़ से पाठ क्षेत्रों को निकालता है, अनुकूलन विकल्पों का उपयोग करके (रेगुलर एक्सप्रेशन, केस मिलान, आदि)।

```csharp
public IEnumerable<PageTextArea> GetTextAreas(PageTextAreaOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| options | PageTextAreaOptions | टेक्स्ट एरिया निष्कर्षण के विकल्प। |

### रिटर्न वैल्यू

एक संग्रह [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) वस्तुओं का; यदि टेक्स्ट एरिया निष्कर्षण समर्थित नहीं है तो `null`।

### टिप्पणियाँ

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Examples

निम्नलिखित उदाहरण दिखाता है कि ऊपरी-बाएँ कोने से केवल अंकों वाले टेक्स्ट एरिया कैसे निकालें:

```csharp
// Parser class का एक instance बनाएं
using(Parser parser = new Parser(filePath))
{
    // टेक्स्ट एरिया निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प बनाएं
    PageTextAreaOptions options = new PageTextAreaOptions("[0-9]+", new Rectangle(new Point(0, 0), new Size(300, 100)));

    // पृष्ठ के ऊपरी-बाएँ कोने से केवल अंकों वाले टेक्स्ट एरिया निकालें:
    IEnumerable<PageTextArea> areas = parser.GetTextAreas(options);
    // जाँचें कि टेक्स्ट एरिया निष्कर्षण समर्थित है या नहीं
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // पृष्ठ टेक्स्ट एरिया पर पुनरावृति करें
    foreach(PageTextArea a in areas)
    {
        // एक पृष्ठ अनुक्रमांक, आयत और टेक्स्ट एरिया मान को प्रिंट करें:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### संबंधित देखें

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(int) {#gettextareas_2}

दस्तावेज़ पृष्ठ से पाठ क्षेत्रों को निकालता है।

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageIndex | Int32 | शून्य-आधारित पेज इंडेक्स। |

### रिटर्न वैल्यू

एक संग्रह [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) वस्तुओं का; यदि टेक्स्ट एरिया निष्कर्षण समर्थित नहीं है तो `null`।

### टिप्पणियाँ

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### Examples

दस्तावेज़ पृष्ठ से टेक्स्ट एरिया निकालने के लिए निम्नलिखित विधि का उपयोग किया जाता है:

```csharp
// Parser class का एक instance बनाएं
using(Parser parser = new Parser(filePath))
{
    // जाँचें कि दस्तावेज़ टेक्स्ट एरिया निष्कर्षण का समर्थन करता है या नहीं
    if(!parser.Features.TextAreas)
    {
        Console.WriteLine("Document isn't supports text areas extraction.");
        return;
    }

    // दस्तावेज़ की जानकारी प्राप्त करें
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // जाँचें कि दस्तावेज़ में पृष्ठ हैं या नहीं
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // पृष्ठों पर इटररेट करें
    for(int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // पृष्ठ संख्या प्रिंट करें 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
 
        // पृष्ठ टेक्स्ट एरिया पर पुनरावृति करें
        // हम null-जाँच को अनदेखा करते हैं क्योंकि हमने पहले टेक्स्ट एरिया निष्कर्षण सुविधा समर्थन की जाँच की थी
        foreach(PageTextArea a in parser.GetTextAreas(pageIndex))
        {
            // एक आयत और टेक्स्ट एरिया मान को प्रिंट करें:
            Console.WriteLine(string.Format("R: {0}, Text: {1}", a.Rectangle, a.Text));
        }
    }
}
```

### संबंधित देखें

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTextAreas(int, PageTextAreaOptions) {#gettextareas_3}

दस्तावेज़ पृष्ठ से पाठ क्षेत्रों को निकालता है, अनुकूलन विकल्पों का उपयोग करके (रेगुलर एक्सप्रेशन, केस मिलान, आदि)।

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex, PageTextAreaOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageIndex | Int32 | शून्य-आधारित पेज इंडेक्स। |
| options | PageTextAreaOptions | टेक्स्ट एरिया निष्कर्षण के विकल्प। |

### रिटर्न वैल्यू

एक संग्रह [`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) वस्तुओं का; यदि टेक्स्ट एरिया निष्कर्षण समर्थित नहीं है तो `null`।

### टिप्पणियाँ

**Learn more:**

* [Extract text areas](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### संबंधित देखें

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
