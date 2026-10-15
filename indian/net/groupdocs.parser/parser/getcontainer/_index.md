---
title: "GetContainer"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "दस्तावेज़ से एक कंटेनर ऑब्जेक्ट निकालता है ताकि उन स्वरूपों के साथ काम किया जा सके जिनमें अटैचमेंट, ZIP आर्काइव आदि होते हैं।"
type: docs
weight: 80
url: /hi/net/groupdocs.parser/parser/getcontainer/
---

## Parser.GetContainer method

संलग्नक, ZIP अभिलेख आदि वाले फ़ॉर्मेट के साथ काम करने के लिए दस्तावेज़ से एक कंटेनर ऑब्जेक्ट निकालता है।

```csharp
public IEnumerable<ContainerItem> GetContainer()
```

### रिटर्न वैल्यू

कंटेनर आइटम्स का संग्रह; `null` यदि कंटेनर निष्कर्षण समर्थित नहीं है।

### टिप्पणियाँ

जाँचने के लिए कि क्या स्वरूप अटैचमेंट निकालने का समर्थन करता है, देखें [Supported Document Formats](https://docs.groupdocs.com/parser/net/supported-document-formats/) (**Extract Containers and Attachments** कॉलम)।

**Learn more:**

* [Extract data from attachments and ZIP archives](https://docs.groupdocs.com/display/parsernet/Extract+data+from+attachments+and+ZIP+archives)
* [Iterate through container items](https://docs.groupdocs.com/display/parsernet/Iterate+through+container+items)
* [Extract attachments from PDF portfolios](https://docs.groupdocs.com/display/parsernet/Extract+attachments+from+PDF+portfolios)
* [Extract attachments from Emails](https://docs.groupdocs.com/display/parsernet/Extract+attachments+from+Emails)
* [Extract emails from Outlook Storage](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+Outlook+Storage)
* [Extract text from ZIP archive files](https://docs.groupdocs.com/display/parsernet/Extract+text+from+ZIP+archive+files)

### Examples

निम्नलिखित उदाहरण दिखाता है कि कंटेनर से अटैचमेंट कैसे निकाले जाएँ:

```csharp
// Parser class का एक instance बनाएं
using(Parser parser = new Parser(filePath))
{
    // कंटेनर से अटैचमेंट निकालें
    IEnumerable<ContainerItem> attachments = parser.GetContainer();
    // जाँचें कि कंटेनर निष्कर्षण समर्थित है या नहीं
    if(attachments == null)
    {
        Console.WriteLine("Container extraction isn't supported");
    }
 
    // संलग्नकों पर पुनरावृत्ति करें
    foreach(ContainerItem item in attachments)
    {
        // आइटम का नाम और आकार प्रिंट करें
        Console.WriteLine(string.Format("{0}: {1}", item.Name, item.Size));
    }
}
```

### संबंधित देखें

* class [ContainerItem](../../../groupdocs.parser.data/containeritem)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
