---
title: "GetImageStream"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "छवि स्ट्रीम लौटाता है।"
type: docs
weight: 40
url: /hi/net/groupdocs.parser.data/pageimagearea/getimagestream/
---

## GetImageStream() {#getimagestream}

छवि स्ट्रीम लौटाता है।

```csharp
public Stream GetImageStream()
```

### रिटर्न वैल्यू

छवि वाला एक स्ट्रीम।

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
        // इमेज स्ट्रीम खोलें
        using (Stream imageStream = image.GetImageStream())
        {
            // इमेज सहेजने के लिए फ़ाइल बनाएं
            using (Stream destStream = File.Create(Guid.NewGuid().ToString() + image.FileType.Extension))
            {
                byte[] buffer = new byte[4096];
                int readed = 0;

                do
                {
                    // इमेज स्ट्रीम से डेटा पढ़ें
                    readed = imageStream.Read(buffer, 0, buffer.Length);

                    if (readed > 0)
                    {
                        // फ़ाइल स्ट्रीम में डेटा लिखें
                        destStream.Write(buffer, 0, readed);
                    }
                }
                while (readed > 0);
            }
        }
    }
}
```

### संबंधित देखें

* class [PageImageArea](../../pageimagearea)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

---

## GetImageStream(ImageOptions) {#getimagestream_1}

विभिन्न प्रारूप में छवि स्ट्रीम लौटाता है।

```csharp
public Stream GetImageStream(ImageOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| options | ImageOptions | इमेज निकालने के लिए उपयोग किए जाने वाले विकल्प। |

### रिटर्न वैल्यू

छवि वाला एक स्ट्रीम।

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
        // इमेज स्ट्रीम खोलें
        using (Stream imageStream = image.GetImageStream(options))
        {
            // इमेज सहेजने के लिए फ़ाइल बनाएं
            using (Stream destStream = File.Create(Guid.NewGuid().ToString() + ".png"))
            {
                byte[] buffer = new byte[4096];
                int readed = 0;

                do
                {
                    // इमेज स्ट्रीम से डेटा पढ़ें
                    readed = imageStream.Read(buffer, 0, buffer.Length);

                    if (readed > 0)
                    {
                        // फ़ाइल स्ट्रीम में डेटा लिखें
                        destStream.Write(buffer, 0, readed);
                    }
                }
                while (readed > 0);
            }
        }
    }
}
```

### संबंधित देखें

* class [ImageOptions](../../../groupdocs.parser.options/imageoptions)
* class [PageImageArea](../../pageimagearea)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
