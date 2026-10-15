---
title: "सहेजें"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "छवि को फ़ाइल में सहेजता है।"
type: docs
weight: 50
url: /hi/net/groupdocs.parser.data/pageimagearea/save/
---

## Save(string) {#save}

छवि को फ़ाइल में सहेजता है।

```csharp
public void Save(string filePath)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | स्ट्रिंग | फ़ाइल का पथ। |

### Examples

निम्नलिखित उदाहरण दिखाता है कि छवियों को फ़ाइलों में कैसे सहेजा जाए:

```csharp
// Parser class का एक instance बनाएं
using (Parser parser = new Parser(filePath))
{
    // दस्तावेज़ से छवियों को निकालें
    IEnumerable<PageImageArea> images = parser.GetImages();
    
    // जाँचें कि छवि निष्कर्षण समर्थित है या नहीं
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }

    // छवियों पर पुनरावृति करें
    foreach (PageImageArea image in images)
    {
        // इमेज को फ़ाइल में सहेजें
        image.Save(Guid.NewGuid().ToString() + image.FileType.Extension);
    }
}
```

### संबंधित देखें

* class [PageImageArea](../../pageimagearea)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

---

## Save(string, ImageOptions) {#save_1}

छवि को विभिन्न प्रारूप में फ़ाइल में सहेजता है।

```csharp
public void Save(string filePath, ImageOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | स्ट्रिंग | फ़ाइल का पथ। |
| options | ImageOptions | इमेज सहेजने के लिए उपयोग किए जाने वाले विकल्प। |

### Examples

निम्नलिखित उदाहरण दिखाता है कि विभिन्न फ़ॉर्मेट में इमेज को फ़ाइलों में कैसे सहेजा जाए:

```csharp
// Parser class का एक instance बनाएं
using (Parser parser = new Parser(filePath))
{
    // दस्तावेज़ से छवियों को निकालें
    IEnumerable<PageImageArea> images = parser.GetImages();
    
    // जाँचें कि छवि निष्कर्षण समर्थित है या नहीं
    if (images == null)
    {
        Console.WriteLine("Page images extraction isn't supported");
        return;
    }

    // PNG फ़ॉर्मेट में इमेज सहेजने के विकल्प बनाएं
    ImageOptions options = new ImageOptions(ImageFormat.Png);
    
    // छवियों पर पुनरावृति करें
    foreach (PageImageArea image in images)
    {
        // इमेज को PNG फ़ाइल में सहेजें
        image.Save(Guid.NewGuid().ToString() + ".png", options);
    }
}
```

### संबंधित देखें

* class [ImageOptions](../../../groupdocs.parser.options/imageoptions)
* class [PageImageArea](../../pageimagearea)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
