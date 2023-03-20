---
title: GetTextAreas
second_title: GroupDocs.Parser .NET API संदर्भ के लिए
description: दस्तवेज़ से पठ क्षेत्रं क नकलत है
type: docs
weight: 160
url: /hi/net/groupdocs.parser/parser/gettextareas/
---
## GetTextAreas() {#gettextareas}

दस्तावेज़ से पाठ क्षेत्रों को निकालता है।

```csharp
public IEnumerable<PageTextArea> GetTextAreas()
```

### प्रतिलाभ की मात्रा

का संग्रह[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) ऑब्जेक्ट्स; `व्यर्थ` यदि टेक्स्ट क्षेत्र निकालना समर्थित नहीं है.

### टिप्पणियों

**और अधिक जानें:**

* [पाठ क्षेत्र निकालें](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### उदाहरण

निम्न उदाहरण दिखाता है कि संपूर्ण दस्तावेज़ से सभी पाठ क्षेत्रों को कैसे निकाला जाए:

```csharp
// पार्सर वर्ग का एक उदाहरण बनाएँ
using(Parser parser = new Parser(filePath))
{
    // पाठ क्षेत्रों को निकालें
    IEnumerable<PageTextArea> areas = parser.GetTextAreas();
    // जांचें कि टेक्स्ट क्षेत्र निष्कर्षण समर्थित है या नहीं
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // पृष्ठ पाठ क्षेत्रों पर पुनरावृति करें
    foreach(PageTextArea a in areas)
    {
        // एक पेज इंडेक्स, आयत और टेक्स्ट एरिया वैल्यू प्रिंट करें:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### यह सभी देखें

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

---

## GetTextAreas(PageTextAreaOptions) {#gettextareas_1}

अनुकूलन विकल्पों (रेगुलर एक्सप्रेशन, मैच केस, आदि) का उपयोग करके दस्तावेज़ से टेक्स्ट क्षेत्र निकालता है।

```csharp
public IEnumerable<PageTextArea> GetTextAreas(PageTextAreaOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| options | PageTextAreaOptions | पाठ क्षेत्र निष्कर्षण के लिए विकल्प। |

### प्रतिलाभ की मात्रा

का संग्रह[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) ऑब्जेक्ट्स; `व्यर्थ` यदि टेक्स्ट क्षेत्र निकालना समर्थित नहीं है.

### टिप्पणियों

**और अधिक जानें:**

* [पाठ क्षेत्र निकालें](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### उदाहरण

निम्न उदाहरण दिखाता है कि केवल ऊपरी-बाएँ कोने से अंकों वाले टेक्स्ट क्षेत्रों को कैसे निकाला जाए:

```csharp
// पार्सर वर्ग का एक उदाहरण बनाएँ
using(Parser parser = new Parser(filePath))
{
    // पाठ क्षेत्र निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प बनाएं
    PageTextAreaOptions options = new PageTextAreaOptions("[0-9]+", new Rectangle(new Point(0, 0), new Size(300, 100)));

    // उन पाठ क्षेत्रों को निकालें जिनमें पृष्ठ के ऊपरी-बाएँ कोने से केवल अंक होते हैं:
    IEnumerable<PageTextArea> areas = parser.GetTextAreas(options);
    // जांचें कि टेक्स्ट क्षेत्र निष्कर्षण समर्थित है या नहीं
    if(areas == null)
    {
        Console.WriteLine("Page text areas extraction isn't supported");
        return;
    }
 
    // पृष्ठ पाठ क्षेत्रों पर पुनरावृति करें
    foreach(PageTextArea a in areas)
    {
        // एक पेज इंडेक्स, आयत और टेक्स्ट एरिया वैल्यू प्रिंट करें:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Text: {2}", a.Page.Index, a.Rectangle, a.Text));
    }
}
```

### यह सभी देखें

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

---

## GetTextAreas(int) {#gettextareas_2}

दस्तावेज़ पृष्ठ से टेक्स्ट क्षेत्र निकालता है.

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageIndex | Int32 | शून्य-आधारित पृष्ठ अनुक्रमणिका। |

### प्रतिलाभ की मात्रा

का संग्रह[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) ऑब्जेक्ट्स; `व्यर्थ` यदि टेक्स्ट क्षेत्र निकालना समर्थित नहीं है.

### टिप्पणियों

**और अधिक जानें:**

* [पाठ क्षेत्र निकालें](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### उदाहरण

दस्तावेज़ पृष्ठ से टेक्स्ट क्षेत्र निकालने के लिए निम्न विधि का उपयोग किया जाता है:

```csharp
// पार्सर वर्ग का एक उदाहरण बनाएँ
using(Parser parser = new Parser(filePath))
{
    // जांचें कि क्या दस्तावेज़ पाठ क्षेत्र निष्कर्षण का समर्थन करता है
    if(!parser.Features.TextAreas)
    {
        Console.WriteLine("Document isn't supports text areas extraction.");
        return;
    }

    // दस्तावेज़ की जानकारी प्राप्त करें
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // जांचें कि क्या दस्तावेज़ में पृष्ठ हैं
    if(documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // पृष्ठों पर पुनरावृति
    for(int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // पेज नंबर प्रिंट करें 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
 
        // पृष्ठ पाठ क्षेत्रों पर पुनरावृति करें
        // हम अशक्त-जाँच को अनदेखा करते हैं क्योंकि हमने पहले पाठ क्षेत्र निष्कर्षण सुविधा समर्थन की जाँच की है
        foreach(PageTextArea a in parser.GetTextAreas(pageIndex))
        {
            // एक आयत और पाठ क्षेत्र मान प्रिंट करें:
            Console.WriteLine(string.Format("R: {0}, Text: {1}", a.Rectangle, a.Text));
        }
    }
}
```

### यह सभी देखें

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

---

## GetTextAreas(int, PageTextAreaOptions) {#gettextareas_3}

अनुकूलन विकल्पों (रेगुलर एक्सप्रेशन, मैच केस, आदि) का उपयोग करके दस्तावेज़ पृष्ठ से पाठ क्षेत्रों को निकालता है।

```csharp
public IEnumerable<PageTextArea> GetTextAreas(int pageIndex, PageTextAreaOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageIndex | Int32 | शून्य-आधारित पृष्ठ अनुक्रमणिका। |
| options | PageTextAreaOptions | पाठ क्षेत्र निष्कर्षण के लिए विकल्प। |

### प्रतिलाभ की मात्रा

का संग्रह[`PageTextArea`](../../../groupdocs.parser.data/pagetextarea) ऑब्जेक्ट्स; `व्यर्थ` यदि टेक्स्ट क्षेत्र निकालना समर्थित नहीं है.

### टिप्पणियों

**और अधिक जानें:**

* [पाठ क्षेत्र निकालें](https://docs.groupdocs.com/display/parsernet/Extract+text+areas)

### यह सभी देखें

* class [PageTextArea](../../../groupdocs.parser.data/pagetextarea)
* class [PageTextAreaOptions](../../../groupdocs.parser.options/pagetextareaoptions)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
