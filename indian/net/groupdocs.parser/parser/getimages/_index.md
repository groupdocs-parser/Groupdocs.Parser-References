---
title: GetImages
second_title: GroupDocs.Parser .NET API संदर्भ के लिए
description: दस्तवेज़ से छवयं क नकलत है
type: docs
weight: 110
url: /hi/net/groupdocs.parser/parser/getimages/
---
## GetImages() {#getimages}

दस्तावेज़ से छवियों को निकालता है।

```csharp
public IEnumerable<PageImageArea> GetImages()
```

### प्रतिलाभ की मात्रा

का संग्रह[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) ऑब्जेक्ट्स; `व्यर्थ` अगर छवि निष्कर्षण समर्थित नहीं है.

### टिप्पणियों

**और अधिक जानें:**

* [दस्तावेजों से छवियां निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [छवियों को फ़ाइलों में निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Microsoft Office Word दस्तावेज़ों से छवियां निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Microsoft Office Excel स्प्रेडशीट से चित्र निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Microsoft Office PowerPoint प्रस्तुतियों से चित्र निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [ईमेल से छवियां निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [पीडीएफ दस्तावेजों से छवियां निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### उदाहरण

निम्न उदाहरण दिखाता है कि संपूर्ण दस्तावेज़ से सभी छवियों को कैसे निकालना है:

```csharp
// पार्सर वर्ग का एक उदाहरण बनाएँ
using (Parser parser = new Parser(filePath))
{
    // छवियों को निकालें
    IEnumerable<PageImageArea> images = parser.GetImages();
    // जांचें कि क्या छवि निष्कर्षण समर्थित है
    if (images == null)
    {
        Console.WriteLine("Images extraction isn't supported");
        return;
    }
    // छवियों पर पुनरावृति
    foreach (PageImageArea image in images)
    {
        // पृष्ठ अनुक्रमणिका, आयत और छवि प्रकार प्रिंट करें:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### यह सभी देखें

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

---

## GetImages(PageAreaOptions) {#getimages_1}

अनुकूलन विकल्पों का उपयोग करके दस्तावेज़ से छवियों को निकालता है (छवियों वाले आयताकार क्षेत्र को सेट करने के लिए)

```csharp
public IEnumerable<PageImageArea> GetImages(PageAreaOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| options | PageAreaOptions | छवि निष्कर्षण के लिए विकल्प। |

### प्रतिलाभ की मात्रा

का संग्रह[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) ऑब्जेक्ट्स; `व्यर्थ` अगर छवि निष्कर्षण समर्थित नहीं है.

### टिप्पणियों

**और अधिक जानें:**

* [दस्तावेजों से छवियां निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [छवियों को फ़ाइलों में निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [दस्तावेज़ पृष्ठ क्षेत्र से छवियां निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Microsoft Office Word दस्तावेज़ों से छवियां निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Microsoft Office Excel स्प्रेडशीट से चित्र निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Microsoft Office PowerPoint प्रस्तुतियों से चित्र निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [ईमेल से छवियां निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [पीडीएफ दस्तावेजों से छवियां निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### उदाहरण

निम्न उदाहरण दिखाता है कि ऊपरी-बाएँ कोने से केवल छवियों को कैसे निकाला जाए:

```csharp
// पार्सर वर्ग का एक उदाहरण बनाएँ
using (Parser parser = new Parser(filePath))
{
    // छवि निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प बनाएं
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(0, 0), new Size(300, 100)));
    // पृष्ठ के ऊपरी-बाएँ कोने से चित्र निकालें:
    IEnumerable<PageImageArea> images = parser.GetImages(options);
    // जांचें कि क्या छवि निष्कर्षण समर्थित है
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }
    // छवियों पर पुनरावृति
    foreach (PageImageArea image in images)
    {
        // पृष्ठ अनुक्रमणिका, आयत और छवि प्रकार प्रिंट करें:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### यह सभी देखें

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

---

## GetImages(int) {#getimages_2}

दस्तावेज़ पृष्ठ से छवियां निकालता है.

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageIndex | Int32 | शून्य-आधारित पृष्ठ अनुक्रमणिका। |

### प्रतिलाभ की मात्रा

का संग्रह[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) ऑब्जेक्ट्स; `व्यर्थ` अगर छवि निष्कर्षण समर्थित नहीं है.

### टिप्पणियों

**और अधिक जानें:**

* [दस्तावेजों से छवियां निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [छवियों को फ़ाइलों में निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [दस्तावेज़ पृष्ठ से छवियां निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Microsoft Office Word दस्तावेज़ों से छवियां निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Microsoft Office Excel स्प्रेडशीट से चित्र निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Microsoft Office PowerPoint प्रस्तुतियों से चित्र निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [ईमेल से छवियां निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [पीडीएफ दस्तावेजों से छवियां निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### उदाहरण

दस्तावेज़ पृष्ठ से छवियां निकालने के लिए निम्न विधि का उपयोग किया जाता है:

```csharp
// पार्सर वर्ग का एक उदाहरण बनाएँ
using (Parser parser = new Parser(filePath))
{
    // जांचें कि क्या दस्तावेज़ छवि निष्कर्षण का समर्थन करता है
    if (!parser.Features.Images)
    {
        Console.WriteLine("Document isn't supports images extraction.");
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
    for (int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // पेज नंबर प्रिंट करें 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // छवियों पर पुनरावृति
        // हम अशक्त-जाँच को अनदेखा करते हैं क्योंकि हमने पहले छवि निष्कर्षण सुविधा समर्थन की जाँच की है
        foreach (PageImageArea image in parser.GetImages(pageIndex))
        {
            // एक आयत और छवि प्रकार प्रिंट करें
            Console.WriteLine(string.Format("R: {0}, Text: {1}", image.Rectangle, image.FileType));
        }
    }
}
```

### यह सभी देखें

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

---

## GetImages(int, PageAreaOptions) {#getimages_3}

अनुकूलन विकल्पों का उपयोग करके दस्तावेज़ पृष्ठ से छवियां निकालता है (आयताकार क्षेत्र सेट करने के लिए जिसमें चित्र शामिल हैं)

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex, PageAreaOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageIndex | Int32 | शून्य-आधारित पृष्ठ अनुक्रमणिका। |
| options | PageAreaOptions | छवि निष्कर्षण के लिए विकल्प। |

### प्रतिलाभ की मात्रा

का संग्रह[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) ऑब्जेक्ट्स; `व्यर्थ` अगर छवि निष्कर्षण समर्थित नहीं है.

### टिप्पणियों

**और अधिक जानें:**

* [दस्तावेजों से छवियां निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [छवियों को फ़ाइलों में निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [दस्तावेज़ पृष्ठ से छवियां निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [दस्तावेज़ पृष्ठ क्षेत्र से छवियां निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Microsoft Office Word दस्तावेज़ों से छवियां निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Microsoft Office Excel स्प्रेडशीट से चित्र निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Microsoft Office PowerPoint प्रस्तुतियों से चित्र निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [ईमेल से छवियां निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [पीडीएफ दस्तावेजों से छवियां निकालें](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### यह सभी देखें

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
