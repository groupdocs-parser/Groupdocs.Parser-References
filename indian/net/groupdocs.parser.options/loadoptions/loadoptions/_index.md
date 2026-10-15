---
title: "LoadOptions"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "LoadOptionsgroupdocs.parser.options/loadoptions क्लास की एक नई इंस्टेंस को खाली Passwordgroupdocs.parser.options/loadoptions/password और FileFormatgroupdocs.parser.options/loadoptions/fileformat को Unknown के बराबर तथा डिफ़ॉल्ट एन्कोडिंग्स के साथ इनिशियलाइज़ करता है।"
type: docs
weight: 10
url: /hi/net/groupdocs.parser.options/loadoptions/loadoptions/
---

## LoadOptions() {#constructor}

[`LoadOptions`](../../loadoptions) क्लास की एक नई इंस्टेंस को खाली [`Password`](../password) और [`FileFormat`](../fileformat) को Unknown के बराबर तथा डिफ़ॉल्ट एन्कोडिंग्स के साथ इनिशियलाइज़ करता है।

```csharp
public LoadOptions()
```

### संबंधित देखें

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(TimeSpan) {#constructor_10}

[`LoadOptions`](../../loadoptions) क्लास की एक नई इंस्टेंस को *timeout* के साथ इनिशियलाइज़ करता है।

```csharp
public LoadOptions(TimeSpan timeout)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| timeout | TimeSpan | वेट करने के लिए मिलीसेकंड की संख्या का प्रतिनिधित्व करने वाला TimeSpan। |

### संबंधित देखें

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(string) {#constructor_9}

[`LoadOptions`](../../loadoptions) क्लास की एक नई इंस्टेंस को [`FileFormat`](../fileformat) को Unknown के बराबर तथा डिफ़ॉल्ट एन्कोडिंग्स के साथ इनिशियलाइज़ करता है।

```csharp
public LoadOptions(string password)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| password | स्ट्रिंग | पासवर्ड-प्रोटेक्टेड फ़ाइल को खोलने के लिए पासवर्ड। |

### संबंधित देखें

* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat) {#constructor_1}

[`LoadOptions`](../../loadoptions) क्लास की एक नई इंस्टेंस को खाली [`Password`](../password) और डिफ़ॉल्ट एन्कोडिंग्स के साथ इनिशियलाइज़ करता है।

```csharp
public LoadOptions(FileFormat fileFormat)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileFormat | FileFormat | फ़ाइल का फ़ॉर्मेट। |

### संबंधित देखें

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string) {#constructor_2}

[`LoadOptions`](../../loadoptions) क्लास की एक नई इंस्टेंस को पासवर्ड और डिफ़ॉल्ट एन्कोडिंग्स के साथ इनिशियलाइज़ करता है।

```csharp
public LoadOptions(FileFormat fileFormat, string password)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileFormat | FileFormat | फ़ाइल का फ़ॉर्मेट। |
| password | स्ट्रिंग | पासवर्ड-प्रोटेक्टेड फ़ाइल को खोलने के लिए पासवर्ड। |

### संबंधित देखें

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding) {#constructor_3}

[`LoadOptions`](../../loadoptions) क्लास की एक नई इंस्टेंस को कस्टम एन्कोडिंग्स के साथ इनिशियलाइज़ करता है।

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileFormat | FileFormat | फ़ाइल का फ़ॉर्मेट। |
| password | स्ट्रिंग | पासवर्ड-प्रोटेक्टेड फ़ाइल को खोलने के लिए पासवर्ड। |
| encoding | Encoding | डॉक्यूमेंट की एन्कोडिंग। |
| defaultAnsiEncoding | Encoding | डिफ़ॉल्ट ANSI एन्कोडिंग जो एन्कोडिंग डिटेक्शन के लिए उपयोग की जाती है। |

### संबंधित देखें

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileFormat, string, Encoding, Encoding, TimeSpan) {#constructor_4}

[`LoadOptions`](../../loadoptions) क्लास की पूरी तरह कस्टमाइज़्ड नई इंस्टेंस को इनिशियलाइज़ करता है।

```csharp
public LoadOptions(FileFormat fileFormat, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding, TimeSpan timeout)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileFormat | FileFormat | फ़ाइल का फ़ॉर्मेट। |
| password | स्ट्रिंग | पासवर्ड-प्रोटेक्टेड फ़ाइल को खोलने के लिए पासवर्ड। |
| encoding | Encoding | डॉक्यूमेंट की एन्कोडिंग। |
| defaultAnsiEncoding | Encoding | डिफ़ॉल्ट ANSI एन्कोडिंग जो एन्कोडिंग डिटेक्शन के लिए उपयोग की जाती है। |
| timeout | TimeSpan | वेट करने के लिए मिलीसेकंड की संख्या का प्रतिनिधित्व करने वाला TimeSpan। |

### संबंधित देखें

* enum [FileFormat](../../fileformat)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType) {#constructor_5}

[`LoadOptions`](../../loadoptions) क्लास की एक नई इंस्टेंस को खाली [`Password`](../password) और डिफ़ॉल्ट एन्कोडिंग्स के साथ इनिशियलाइज़ करता है।

```csharp
public LoadOptions(FileType fileType)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileType | FileType | फ़ाइल का प्रकार। |

### संबंधित देखें

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string) {#constructor_6}

[`LoadOptions`](../../loadoptions) क्लास की एक नई इंस्टेंस को पासवर्ड और डिफ़ॉल्ट एन्कोडिंग्स के साथ इनिशियलाइज़ करता है।

```csharp
public LoadOptions(FileType fileType, string password)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileType | FileType | फ़ाइल का प्रकार। |
| password | स्ट्रिंग | पासवर्ड-प्रोटेक्टेड फ़ाइल को खोलने के लिए पासवर्ड। |

### संबंधित देखें

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string, Encoding, Encoding) {#constructor_7}

[`LoadOptions`](../../loadoptions) क्लास की एक नई इंस्टेंस को कस्टम एन्कोडिंग्स के साथ इनिशियलाइज़ करता है।

```csharp
public LoadOptions(FileType fileType, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileType | FileType | फ़ाइल का प्रकार। |
| password | स्ट्रिंग | पासवर्ड-प्रोटेक्टेड फ़ाइल को खोलने के लिए पासवर्ड। |
| encoding | Encoding | डॉक्यूमेंट की एन्कोडिंग। |
| defaultAnsiEncoding | Encoding | डिफ़ॉल्ट ANSI एन्कोडिंग जो एन्कोडिंग डिटेक्शन के लिए उपयोग की जाती है। |

### संबंधित देखें

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

---

## LoadOptions(FileType, string, Encoding, Encoding, TimeSpan) {#constructor_8}

[`LoadOptions`](../../loadoptions) क्लास की पूरी तरह कस्टमाइज़्ड नई इंस्टेंस को इनिशियलाइज़ करता है।

```csharp
public LoadOptions(FileType fileType, string password, Encoding encoding, 
    Encoding defaultAnsiEncoding, TimeSpan timeout)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| fileType | FileType | फ़ाइल का प्रकार। |
| password | स्ट्रिंग | पासवर्ड-प्रोटेक्टेड फ़ाइल को खोलने के लिए पासवर्ड। |
| encoding | Encoding | डॉक्यूमेंट की एन्कोडिंग। |
| defaultAnsiEncoding | Encoding | डिफ़ॉल्ट ANSI एन्कोडिंग जो एन्कोडिंग डिटेक्शन के लिए उपयोग की जाती है। |
| timeout | TimeSpan | वेट करने के लिए मिलीसेकंड की संख्या का प्रतिनिधित्व करने वाला TimeSpan। |

### संबंधित देखें

* class [FileType](../../filetype)
* class [LoadOptions](../../loadoptions)
* namespace [GroupDocs.Parser.Options](../../../groupdocs.parser.options)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
