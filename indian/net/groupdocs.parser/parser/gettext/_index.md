---
title: GetText
second_title: GroupDocs.Parser .NET API संदर्भ के लिए
description: दस्तवेज़ से टेक्स्ट नकलत है.
type: docs
weight: 150
url: /hi/net/groupdocs.parser/parser/gettext/
---
## GetText() {#gettext}

दस्तावेज़ से टेक्स्ट निकालता है.

```csharp
public TextReader GetText()
```

### प्रतिलाभ की मात्रा

का एक उदाहरणTextReader निकाले गए पाठ के साथ कक्षा; `व्यर्थ` यदि पाठ निष्कर्षण समर्थित नहीं है.

### टिप्पणियों

**और अधिक जानें:**

* [दस्तावेज़ों से पाठ निकालें](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [सटीक मोड में टेक्स्ट निकालें](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### उदाहरण

निम्न उदाहरण दिखाता है कि किसी दस्तावेज़ से पाठ कैसे निकालना है:

```csharp
// पार्सर वर्ग का एक उदाहरण बनाएँ
using(Parser parser = new Parser(filePath))
{
    // पाठक में एक पाठ निकालें
    using(TextReader reader = parser.GetText())
    {
        // दस्तावेज़ से एक पाठ प्रिंट करें
        // यदि पाठ निष्कर्षण समर्थित नहीं है, तो एक पाठक शून्य है
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### यह सभी देखें

* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

---

## GetText(TextOptions) {#gettext_1}

पाठ विकल्पों का उपयोग करके दस्तावेज़ से एक पाठ पृष्ठ निकालता है (कच्चे तेज़ पाठ निष्कर्षण मोड को सक्षम करने के लिए)।

```csharp
public TextReader GetText(TextOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| options | TextOptions | पाठ निष्कर्षण विकल्प। |

### प्रतिलाभ की मात्रा

का एक उदाहरणTextReader निकाले गए पाठ के साथ कक्षा; `व्यर्थ` यदि पाठ निष्कर्षण समर्थित नहीं है.

### टिप्पणियों

**और अधिक जानें:**

* [सटीक मोड में टेक्स्ट निकालें](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [रॉ मोड में टेक्स्ट निकालें](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### उदाहरण

निम्न उदाहरण दिखाता है कि किसी दस्तावेज़ से कच्चे पाठ को कैसे निकालना है:

```csharp
// पार्सर वर्ग का एक उदाहरण बनाएँ
using(Parser parser = new Parser(filePath))
{
    // पाठक में एक कच्चा पाठ निकालें
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // दस्तावेज़ से एक पाठ प्रिंट करें
        // यदि पाठ निष्कर्षण समर्थित नहीं है, तो एक पाठक शून्य है
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### यह सभी देखें

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

---

## GetText(int) {#gettext_2}

दस्तावेज़ पृष्ठ से टेक्स्ट निकालता है.

```csharp
public TextReader GetText(int pageIndex)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageIndex | Int32 | शून्य-आधारित पृष्ठ अनुक्रमणिका। |

### प्रतिलाभ की मात्रा

का एक उदाहरणTextReader निकाले गए पाठ के साथ कक्षा; `व्यर्थ` यदि पाठ पृष्ठ निकालना समर्थित नहीं है.

### टिप्पणियों

**और अधिक जानें:**

* [सटीक मोड में टेक्स्ट निकालें](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### उदाहरण

निम्न उदाहरण दिखाता है कि दस्तावेज़ पृष्ठ से टेक्स्ट कैसे निकाला जाए:

```csharp
// पार्सर वर्ग का एक उदाहरण बनाएँ
using(Parser parser = new Parser(filePath))
{
    // जांचें कि दस्तावेज़ टेक्स्ट निष्कर्षण का समर्थन करता है या नहीं
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
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
    for(int p = 0; p<documentInfo.PageCount; p++)
    {
        // पेज नंबर प्रिंट करें 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
 
        // पाठक में एक पाठ निकालें
        using(TextReader reader = parser.GetText(p))
        {
            // दस्तावेज़ से एक पाठ प्रिंट करें
            // हम अशक्त-जाँच को अनदेखा करते हैं क्योंकि हमने पहले पाठ निष्कर्षण सुविधा समर्थन की जाँच की है
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### यह सभी देखें

* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

---

## GetText(int, TextOptions) {#gettext_3}

पाठ विकल्पों का उपयोग करके दस्तावेज़ पृष्ठ से एक पाठ निकालता है (कच्चे तेज़ पाठ निष्कर्षण मोड को सक्षम करने के लिए)।

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageIndex | Int32 | शून्य-आधारित पृष्ठ अनुक्रमणिका। |
| options | TextOptions | पाठ निष्कर्षण विकल्प। |

### प्रतिलाभ की मात्रा

का एक उदाहरणTextReader निकाले गए पाठ के साथ कक्षा; `व्यर्थ` यदि पाठ पृष्ठ निकालना समर्थित नहीं है.

### टिप्पणियों

**और अधिक जानें:**

* [सटीक मोड में टेक्स्ट निकालें](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [रॉ मोड में टेक्स्ट निकालें](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### उदाहरण

निम्न उदाहरण दिखाता है कि दस्तावेज़ पृष्ठ से कच्चे पाठ को कैसे निकाला जाए:

```csharp
// पार्सर वर्ग का एक उदाहरण बनाएँ
using(Parser parser = new Parser(filePath))
{
    // जांचें कि दस्तावेज़ टेक्स्ट निष्कर्षण का समर्थन करता है या नहीं
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // दस्तावेज़ की जानकारी प्राप्त करें
    DocumentInfo documentInfo = parser.GetDocumentInfo() as DocumentInfo;
    // जांचें कि क्या दस्तावेज़ में पृष्ठ हैं
    if(documentInfo == null || documentInfo.RawPageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // पृष्ठों पर पुनरावृति
    for(int p = 0; p<documentInfo.RawPageCount; p++)
    {
        // पेज नंबर प्रिंट करें 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.RawPageCount));
 
        // पाठक में एक पाठ निकालें
        using(TextReader reader = parser.GetText(p, new TextOptions(true)))
        {
            // दस्तावेज़ से एक पाठ प्रिंट करें
            // हम अशक्त-जाँच को अनदेखा करते हैं क्योंकि हमने पहले पाठ निष्कर्षण सुविधा समर्थन की जाँच की है
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### यह सभी देखें

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
