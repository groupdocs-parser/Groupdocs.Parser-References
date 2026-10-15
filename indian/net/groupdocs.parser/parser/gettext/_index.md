---
title: "GetText"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "दस्तावेज़ से पाठ निकालता है।"
type: docs
weight: 180
url: /hi/net/groupdocs.parser/parser/gettext/
---

## GetText() {#gettext}

दस्तावेज़ से पाठ निकालता है।

```csharp
public TextReader GetText()
```

### रिटर्न वैल्यू

एक TextReader क्लास का उदाहरण जिसमें निकाला गया पाठ है; यदि पाठ निष्कर्षण समर्थित नहीं है तो `null`।

### टिप्पणियाँ

**Learn more:**

* [Extract text from documents](https://docs.groupdocs.com/display/parsernet/Extract+text+from+documents)
* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Examples

निम्नलिखित उदाहरण दिखाता है कि दस्तावेज़ से पाठ कैसे निकाला जाए:

```csharp
// Parser class का एक instance बनाएं
using(Parser parser = new Parser(filePath))
{
    // पाठ को रीडर में निकालें
    using(TextReader reader = parser.GetText())
    {
        // दस्तावेज़ से पाठ प्रिंट करें
        // यदि पाठ निष्कर्षण समर्थित नहीं है, तो रीडर `null` होगा
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### संबंधित देखें

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(TextOptions) {#gettext_1}

दस्तावेज़ से पाठ पृष्ठ निकालता है, पाठ विकल्पों का उपयोग करके (कच्चा तेज़ पाठ निष्कर्षण मोड सक्षम करने के लिए)।

```csharp
public TextReader GetText(TextOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| options | TextOptions | पाठ निष्कर्षण विकल्प। |

### रिटर्न वैल्यू

एक TextReader क्लास का उदाहरण जिसमें निकाला गया पाठ है; यदि पाठ निष्कर्षण समर्थित नहीं है तो `null`।

### टिप्पणियाँ

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Examples

निम्नलिखित उदाहरण दिखाता है कि दस्तावेज़ से कच्चा पाठ कैसे निकाला जाए:

```csharp
// Parser class का एक instance बनाएं
using(Parser parser = new Parser(filePath))
{
    // कच्चा पाठ रीडर में निकालें
    using(TextReader reader = parser.GetText(new TextOptions(true)))
    {
        // दस्तावेज़ से पाठ प्रिंट करें
        // यदि पाठ निष्कर्षण समर्थित नहीं है, तो रीडर `null` होगा
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### संबंधित देखें

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(int) {#gettext_2}

दस्तावेज़ पृष्ठ से पाठ निकालता है।

```csharp
public TextReader GetText(int pageIndex)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageIndex | Int32 | शून्य-आधारित पेज इंडेक्स। |

### रिटर्न वैल्यू

एक TextReader क्लास का उदाहरण जिसमें निकाला गया पाठ है; यदि पाठ पृष्ठ निष्कर्षण समर्थित नहीं है तो `null`।

### टिप्पणियाँ

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)

### Examples

निम्नलिखित उदाहरण दिखाता है कि दस्तावेज़ पृष्ठ से पाठ कैसे निकाला जाए:

```csharp
// Parser class का एक instance बनाएं
using(Parser parser = new Parser(filePath))
{
    // जाँचें कि दस्तावेज़ पाठ निष्कर्षण का समर्थन करता है या नहीं
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
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
    for(int p = 0; p<documentInfo.PageCount; p++)
    {
        // पृष्ठ संख्या प्रिंट करें 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
 
        // पाठ को रीडर में निकालें
        using(TextReader reader = parser.GetText(p))
        {
            // दस्तावेज़ से पाठ प्रिंट करें
            // हम null-चेकिंग को अनदेखा करते हैं क्योंकि हमने पहले ही पाठ निष्कर्षण सुविधा समर्थन की जाँच कर ली है
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### संबंधित देखें

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetText(int, TextOptions) {#gettext_3}

दस्तावेज़ पृष्ठ से पाठ निकालता है, पाठ विकल्पों का उपयोग करके (कच्चा तेज़ पाठ निष्कर्षण मोड सक्षम करने के लिए)।

```csharp
public TextReader GetText(int pageIndex, TextOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageIndex | Int32 | शून्य-आधारित पेज इंडेक्स। |
| options | TextOptions | पाठ निष्कर्षण विकल्प। |

### रिटर्न वैल्यू

एक TextReader क्लास का उदाहरण जिसमें निकाला गया पाठ है; यदि पाठ पृष्ठ निष्कर्षण समर्थित नहीं है तो `null`।

### टिप्पणियाँ

**Learn more:**

* [Extract text in Accurate mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Accurate+mode)
* [Extract text in Raw mode](https://docs.groupdocs.com/display/parsernet/Extract+text+in+Raw+mode)

### Examples

निम्नलिखित उदाहरण दिखाता है कि दस्तावेज़ पृष्ठ से कच्चा पाठ कैसे निकाला जाए:

```csharp
// Parser class का एक instance बनाएं
using(Parser parser = new Parser(filePath))
{
    // जाँचें कि दस्तावेज़ पाठ निष्कर्षण का समर्थन करता है या नहीं
    if(!parser.Features.Text)
    {
        Console.WriteLine("Document isn't supports text extraction.");
        return;
    }

    // दस्तावेज़ की जानकारी प्राप्त करें
    DocumentInfo documentInfo = parser.GetDocumentInfo() as DocumentInfo;
    // जाँचें कि दस्तावेज़ में पृष्ठ हैं या नहीं
    if(documentInfo == null || documentInfo.RawPageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
 
    // पृष्ठों पर इटररेट करें
    for(int p = 0; p<documentInfo.RawPageCount; p++)
    {
        // पृष्ठ संख्या प्रिंट करें 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.RawPageCount));
 
        // पाठ को रीडर में निकालें
        using(TextReader reader = parser.GetText(p, new TextOptions(true)))
        {
            // दस्तावेज़ से पाठ प्रिंट करें
            // हम null-चेकिंग को अनदेखा करते हैं क्योंकि हमने पहले ही पाठ निष्कर्षण सुविधा समर्थन की जाँच कर ली है
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### संबंधित देखें

* class [TextOptions](../../../groupdocs.parser.options/textoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
