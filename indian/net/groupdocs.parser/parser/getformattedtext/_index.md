---
title: "GetFormattedText"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "दस्तावेज़ से फ़ॉर्मेटेड टेक्स्ट निकालता है।"
type: docs
weight: 100
url: /hi/net/groupdocs.parser/parser/getformattedtext/
---

## GetFormattedText(FormattedTextOptions) {#getformattedtext}

दस्तावेज़ से फ़ॉर्मेटेड टेक्स्ट निकालता है।

```csharp
public TextReader GetFormattedText(FormattedTextOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| options | FormattedTextOptions | फ़ॉर्मेटेड टेक्स्ट निष्कर्षण विकल्प। |

### रिटर्न वैल्यू

एक TextReader क्लास का उदाहरण जिसमें निकाला गया टेक्स्ट होता है; `null` यदि फ़ॉर्मेटेड टेक्स्ट निष्कर्षण समर्थित नहीं है।

### टिप्पणियाँ

**Learn more:**

* [Extract formatted text from document](https://docs.groupdocs.com/display/parsernet/Extract+formatted+text+from+document)
* Extract a document text as [HTML](https://docs.groupdocs.com/display/parsernet/HTML)
* Extract a document text as [Markdown](https://docs.groupdocs.com/display/parsernet/Markdown)
* Extract a document text as [Plain text](https://docs.groupdocs.com/display/parsernet/Plain+text)

### Examples

निम्नलिखित उदाहरण दिखाता है कि दस्तावेज़ टेक्स्ट को HTML टेक्स्ट के रूप में कैसे निकाला जाए:

```csharp
// Parser class का एक instance बनाएं
using (Parser parser = new Parser(filePath))
{
    // फ़ॉर्मेटेड टेक्स्ट को रीडर में निकालें
    using (TextReader reader = parser.GetFormattedText(new FormattedTextOptions(FormattedTextMode.Html)))
    {
        // दस्तावेज़ से फ़ॉर्मेटेड टेक्स्ट प्रिंट करें
        // यदि फ़ॉर्मेटेड टेक्स्ट निष्कर्षण समर्थित नहीं है, तो रीडर null होता है
        Console.WriteLine(reader == null ? "Formatted text extraction isn't suppported" : reader.ReadToEnd());
    }
}
```

### संबंधित देखें

* class [FormattedTextOptions](../../../groupdocs.parser.options/formattedtextoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetFormattedText(int, FormattedTextOptions) {#getformattedtext_1}

दस्तावेज़ पृष्ठ से फ़ॉर्मेटेड टेक्स्ट निकालता है।

```csharp
public TextReader GetFormattedText(int pageIndex, FormattedTextOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageIndex | Int32 | शून्य-आधारित पेज इंडेक्स। |
| options | FormattedTextOptions | फ़ॉर्मेटेड टेक्स्ट निष्कर्षण विकल्प। |

### रिटर्न वैल्यू

एक TextReader क्लास का उदाहरण जिसमें निकाला गया टेक्स्ट होता है; `null` यदि फ़ॉर्मेटेड टेक्स्ट पृष्ठ निष्कर्षण समर्थित नहीं है।

### टिप्पणियाँ

**Learn more:**

* [Extract formatted text from document page](https://docs.groupdocs.com/display/parsernet/Extract+formatted+text+from+document+page)
* Extract a document text as [HTML](https://docs.groupdocs.com/display/parsernet/HTML)
* Extract a document text as [Markdown](https://docs.groupdocs.com/display/parsernet/Markdown)
* Extract a document text as [Plain text](https://docs.groupdocs.com/display/parsernet/Plain+text)

### Examples

निम्नलिखित उदाहरण दिखाता है कि दस्तावेज़ पृष्ठ टेक्स्ट को Markdown टेक्स्ट के रूप में कैसे निकाला जाए:

```csharp
// Parser class का एक instance बनाएं
using (Parser parser = new Parser(filePath))
{
    // जाँचें कि दस्तावेज़ फ़ॉर्मेटेड टेक्स्ट निष्कर्षण का समर्थन करता है या नहीं
    if (!parser.Features.FormattedText)
    {
        Console.WriteLine("Document isn't supports formatted text extraction.");
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
    for (int p = 0; p<documentInfo.PageCount; p++)
    {
        // पृष्ठ संख्या प्रिंट करें 
        Console.WriteLine(string.Format("Page {0}/{1}", p + 1, documentInfo.PageCount));
        // फ़ॉर्मेटेड टेक्स्ट को रीडर में निकालें
        using (TextReader reader = parser.GetFormattedText(p, new FormattedTextOptions(FormattedTextMode.Markdown)))
        {
            // दस्तावेज़ से फ़ॉर्मेटेड टेक्स्ट प्रिंट करें
            // हम null-जाँच को अनदेखा करते हैं क्योंकि हमने पहले फ़ॉर्मेटेड टेक्स्ट निष्कर्षण सुविधा समर्थन की जाँच की है
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### संबंधित देखें

* class [FormattedTextOptions](../../../groupdocs.parser.options/formattedtextoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
