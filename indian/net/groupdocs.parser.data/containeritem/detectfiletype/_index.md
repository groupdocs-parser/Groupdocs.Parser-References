---
title: "DetectFileType"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "कंटेनर आइटम की फ़ाइल प्रकार का पता लगाता है।"
type: docs
weight: 60
url: /hi/net/groupdocs.parser.data/containeritem/detectfiletype/
---

## ContainerItem.DetectFileType method

कंटेनर आइटम की फ़ाइल प्रकार का पता लगाता है।

```csharp
public FileType DetectFileType(FileTypeDetectionMode detectionMode)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| detectionMode | FileTypeDetectionMode | फ़ाइल प्रकार पहचान के मोड को परिभाषित करता है। |

### रिटर्न वैल्यू

एक instance of [`FileType`](../../../groupdocs.parser.options/filetype) क्लास; यदि फ़ाइल प्रकार का पता नहीं चलता है तो [`Unknown`](../../../groupdocs.parser.options/filetype/unknown)।

### टिप्पणियाँ

*detectionMode* parameter provides the ability to control file type detection:

* **Default**. The file type is detected by the file extension; if the file extension isn't recognized, the file type is detected by the file content.
* **Extension**.The file type is detected only by the file extension.
* **Content**. The file type is detected only by the file content.

### Examples

निम्नलिखित उदाहरण दिखाता है कि कंटेनर आइटम का फ़ाइल प्रकार कैसे पता किया जाए:

```csharp
// Parser class का एक instance बनाएं
using (Parser parser = new Parser(filePath))
{
    // कंटेनर से अटैचमेंट निकालें
    IEnumerable<ContainerItem> attachments = parser.GetContainer();
    // जाँचें कि कंटेनर निष्कर्षण समर्थित है या नहीं
    if (attachments == null)
    {
        Console.WriteLine("Container extraction isn't supported");
    }
    // संलग्नकों पर पुनरावृत्ति करें
    foreach (ContainerItem item in attachments)
    {
        // फ़ाइल प्रकार का पता लगाएँ
        Options.FileType fileType = item.DetectFileType(Options.FileTypeDetectionMode.Default);

        // नाम और फ़ाइल प्रकार प्रिंट करें
        Console.WriteLine(string.Format("{0}: {1}", item.Name, fileType));
    }
}
```

### संबंधित देखें

* class [FileType](../../../groupdocs.parser.options/filetype)
* enum [FileTypeDetectionMode](../../../groupdocs.parser.options/filetypedetectionmode)
* class [ContainerItem](../../containeritem)
* namespace [GroupDocs.Parser.Data](../../../groupdocs.parser.data)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
