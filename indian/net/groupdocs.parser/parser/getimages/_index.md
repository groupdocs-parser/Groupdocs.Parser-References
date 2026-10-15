---
title: "GetImages"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "दस्तावेज़ से छवियां निकालता है।"
type: docs
weight: 130
url: /hi/net/groupdocs.parser/parser/getimages/
---

## GetImages() {#getimages}

दस्तावेज़ से छवियां निकालता है।

```csharp
public IEnumerable<PageImageArea> GetImages()
```

### रिटर्न वैल्यू

[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) वस्तुओं का संग्रह; `null` यदि छवि निष्कर्षण समर्थित नहीं है।

### टिप्पणियाँ

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Examples

निम्नलिखित उदाहरण दिखाता है कि पूरे दस्तावेज़ से सभी छवियों को कैसे निकाला जाए:

```csharp
// Parser class का एक instance बनाएं
using (Parser parser = new Parser(filePath))
{
    // छवियों को निकालें
    IEnumerable<PageImageArea> images = parser.GetImages();
    // जाँचें कि छवि निष्कर्षण समर्थित है या नहीं
    if (images == null)
    {
        Console.WriteLine("Images extraction isn't supported");
        return;
    }
    // छवियों पर पुनरावृति करें
    foreach (PageImageArea image in images)
    {
        // पृष्ठ सूचकांक, आयत और छवि प्रकार प्रिंट करें:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### संबंधित देखें

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(PageAreaOptions) {#getimages_1}

कस्टमाइज़ेशन विकल्पों का उपयोग करके दस्तावेज़ से छवियां निकालता है (छवियों वाले आयताकार क्षेत्र को सेट करने के लिए)।

```csharp
public IEnumerable<PageImageArea> GetImages(PageAreaOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| options | PageAreaOptions | छवि निष्कर्षण के विकल्प। |

### रिटर्न वैल्यू

[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) वस्तुओं का संग्रह; `null` यदि छवि निष्कर्षण समर्थित नहीं है।

### टिप्पणियाँ

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from document page area](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Examples

निम्नलिखित उदाहरण दिखाता है कि ऊपरी-बाएँ कोने से केवल छवियों को कैसे निकाला जाए:

```csharp
// Parser class का एक instance बनाएं
using (Parser parser = new Parser(filePath))
{
    // छवि निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प बनाएं
    PageAreaOptions options = new PageAreaOptions(new Rectangle(new Point(0, 0), new Size(300, 100)));
    // पृष्ठ के ऊपरी-बाएँ कोने से छवियों को निकालें:
    IEnumerable<PageImageArea> images = parser.GetImages(options);
    // जाँचें कि छवि निष्कर्षण समर्थित है या नहीं
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }
    // छवियों पर पुनरावृति करें
    foreach (PageImageArea image in images)
    {
        // पृष्ठ सूचकांक, आयत और छवि प्रकार प्रिंट करें:
        Console.WriteLine(string.Format("Page: {0}, R: {1}, Type: {2}", image.Page.Index, image.Rectangle, image.FileType));
    }
}
```

### संबंधित देखें

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(int) {#getimages_2}

दस्तावेज़ पृष्ठ से छवियां निकालता है।

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageIndex | Int32 | शून्य-आधारित पेज इंडेक्स। |

### रिटर्न वैल्यू

[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) वस्तुओं का संग्रह; `null` यदि छवि निष्कर्षण समर्थित नहीं है।

### टिप्पणियाँ

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from document page](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### Examples

दस्तावेज़ पृष्ठ से छवियों को निकालने के लिए निम्न विधि का उपयोग किया जाता है:

```csharp
// Parser class का एक instance बनाएं
using (Parser parser = new Parser(filePath))
{
    // जाँचें कि क्या दस्तावेज़ छवियों के निष्कर्षण का समर्थन करता है
    if (!parser.Features.Images)
    {
        Console.WriteLine("Document isn't supports images extraction.");
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
    for (int pageIndex = 0; pageIndex<documentInfo.PageCount; pageIndex++)
    {
        // पृष्ठ संख्या प्रिंट करें 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // छवियों पर पुनरावृति करें
        // हम null-जाँच को नज़रअंदाज़ करते हैं क्योंकि हमने पहले ही छवियों के निष्कर्षण सुविधा समर्थन की जाँच कर ली है
        foreach (PageImageArea image in parser.GetImages(pageIndex))
        {
            // एक आयत और छवि प्रकार प्रिंट करें
            Console.WriteLine(string.Format("R: {0}, Text: {1}", image.Rectangle, image.FileType));
        }
    }
}
```

### संबंधित देखें

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetImages(int, PageAreaOptions) {#getimages_3}

कस्टमाइज़ेशन विकल्पों का उपयोग करके दस्तावेज़ पृष्ठ से छवियां निकालता है (छवियों वाले आयताकार क्षेत्र को सेट करने के लिए)।

```csharp
public IEnumerable<PageImageArea> GetImages(int pageIndex, PageAreaOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageIndex | Int32 | शून्य-आधारित पेज इंडेक्स। |
| options | PageAreaOptions | छवि निष्कर्षण के विकल्प। |

### रिटर्न वैल्यू

[`PageImageArea`](../../../groupdocs.parser.data/pageimagearea) वस्तुओं का संग्रह; `null` यदि छवि निष्कर्षण समर्थित नहीं है।

### टिप्पणियाँ

**Learn more:**

* [Extract images from documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+documents)
* [Extract images to files](https://docs.groupdocs.com/display/parsernet/Extract+images+to+files)
* [Extract images from document page](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page)
* [Extract images from document page area](https://docs.groupdocs.com/display/parsernet/Extract+images+from+document+page+area)
* [Extract images from Microsoft Office Word documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Word+documents)
* [Extract images from Microsoft Office Excel spreadsheets](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+Excel+spreadsheets)
* [Extract images from Microsoft Office PowerPoint presentations](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Microsoft+Office+PowerPoint+presentations)
* [Extract images from Emails](https://docs.groupdocs.com/display/parsernet/Extract+images+from+Emails)
* [Extract images from PDF documents](https://docs.groupdocs.com/display/parsernet/Extract+images+from+PDF+documents)

### संबंधित देखें

* class [PageImageArea](../../../groupdocs.parser.data/pageimagearea)
* class [PageAreaOptions](../../../groupdocs.parser.options/pageareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
