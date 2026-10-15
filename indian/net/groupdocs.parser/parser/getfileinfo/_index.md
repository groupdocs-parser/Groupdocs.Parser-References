---
title: "GetFileInfo"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "फ़ाइल के बारे में सामान्य जानकारी लौटाता है।"
type: docs
weight: 260
url: /hi/net/groupdocs.parser/parser/getfileinfo/
---

## GetFileInfo(string) {#getfileinfo_2}

फ़ाइल के बारे में सामान्य जानकारी लौटाता है।

```csharp
public static FileInfo GetFileInfo(string filePath)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | स्ट्रिंग | फ़ाइल का पथ। |

### रिटर्न वैल्यू

[`FileInfo`](../../../groupdocs.parser.options/fileinfo) क्लास का एक उदाहरण।

### Examples

निम्न कोड दिखाता है कि कैसे जाँचें कि फ़ाइल पासवर्ड-संरक्षित है या नहीं:

```csharp
// फ़ाइल जानकारी प्राप्त करें
Options.FileInfo info = Parser.GetFileInfo(filePath);
// IsEncrypted प्रॉपर्टी जाँचें
Console.WriteLine(info.IsEncrypted ? "Password is required" : "");
```

### संबंधित देखें

* class [FileInfo](../../../groupdocs.parser.options/fileinfo)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetFileInfo(string, LoadOptions) {#getfileinfo_3}

फ़ाइल के बारे में सामान्य जानकारी लौटाता है।

```csharp
public static FileInfo GetFileInfo(string filePath, LoadOptions loadOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | स्ट्रिंग | फ़ाइल का पथ। |
| loadOptions | LoadOptions | फ़ाइल खोलने के विकल्प। |

### रिटर्न वैल्यू

[`FileInfo`](../../../groupdocs.parser.options/fileinfo) क्लास का एक उदाहरण।

### Examples

निम्न कोड दिखाता है कि कैसे पासवर्ड-संरक्षित दस्तावेज़ की फ़ाइल प्रकार जाँचें:

```csharp
// फ़ाइल जानकारी प्राप्त करें
Options.FileInfo info = Parser.GetFileInfo(filePath, new LoadOptions("password"));
// IsEncrypted प्रॉपर्टी जाँचें
Console.WriteLine(info.IsEncrypted ? "Password is required" : "");
// फ़ाइल प्रकार प्रिंट करें
Console.WriteLine(info.FileType.ToString());
```

### संबंधित देखें

* class [FileInfo](../../../groupdocs.parser.options/fileinfo)
* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetFileInfo(Stream) {#getfileinfo}

फ़ाइल के बारे में सामान्य जानकारी लौटाता है।

```csharp
public static FileInfo GetFileInfo(Stream document)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| दस्तावेज़ | Stream | स्रोत इनपुट स्ट्रीम। |

### रिटर्न वैल्यू

[`FileInfo`](../../../groupdocs.parser.options/fileinfo) क्लास का एक उदाहरण।

### Examples

निम्न कोड दिखाता है कि कैसे जाँचें कि फ़ाइल पासवर्ड-संरक्षित है या नहीं:

```csharp
// फ़ाइल जानकारी प्राप्त करें
Options.FileInfo info = Parser.GetFileInfo(document);
// IsEncrypted प्रॉपर्टी जाँचें
Console.WriteLine(info.IsEncrypted ? "Password is required" : "");
```

### संबंधित देखें

* class [FileInfo](../../../groupdocs.parser.options/fileinfo)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetFileInfo(Stream, LoadOptions) {#getfileinfo_1}

फ़ाइल के बारे में सामान्य जानकारी लौटाता है।

```csharp
public static FileInfo GetFileInfo(Stream document, LoadOptions loadOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| दस्तावेज़ | Stream | स्रोत इनपुट स्ट्रीम। |
| loadOptions | LoadOptions | फ़ाइल खोलने के विकल्प। |

### रिटर्न वैल्यू

[`FileInfo`](../../../groupdocs.parser.options/fileinfo) क्लास का एक उदाहरण।

### Examples

निम्न कोड दिखाता है कि कैसे पासवर्ड-संरक्षित दस्तावेज़ की फ़ाइल प्रकार जाँचें:

```csharp
// फ़ाइल जानकारी प्राप्त करें
Options.FileInfo info = Parser.GetFileInfo(document);
// IsEncrypted प्रॉपर्टी जाँचें
Console.WriteLine(info.IsEncrypted ? "Password is required" : "");
// फ़ाइल प्रकार प्रिंट करें
Console.WriteLine(info.FileType.ToString());
```

### संबंधित देखें

* class [FileInfo](../../../groupdocs.parser.options/fileinfo)
* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
