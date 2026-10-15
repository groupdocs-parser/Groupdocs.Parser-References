---
title: "GetBarcodes"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "दस्तावेज़ से बारकोड निकालता है।"
type: docs
weight: 70
url: /hi/net/groupdocs.parser/parser/getbarcodes/
---

## GetBarcodes() {#getbarcodes}

दस्तावेज़ से बारकोड निकालता है।

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes()
```

### रिटर्न वैल्यू

[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) ऑब्जेक्ट्स का संग्रह; `null` यदि बारकोड निष्कर्षण समर्थित नहीं है।

### Examples

निम्न उदाहरण दिखाता है कि दस्तावेज़ से बारकोड कैसे निकाले जाएँ:

```csharp
// Parser class का एक instance बनाएं
using (Parser parser = new Parser(filePath))
{
    // दस्तावेज़ से बारकोड निकालें।
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes();

    // बारकोड पर इटररेट करें
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // पृष्ठ सूचकांक प्रिंट करें
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // बारकोड मान प्रिंट करें
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### संबंधित देखें

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(int) {#getbarcodes_3}

दस्तावेज़ पृष्ठ से बारकोड निकालता है।

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageIndex | Int32 | शून्य-आधारित पेज इंडेक्स। |

### रिटर्न वैल्यू

[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) ऑब्जेक्ट्स का संग्रह; `null` यदि बारकोड निष्कर्षण समर्थित नहीं है।

### Examples

निम्न उदाहरण दिखाता है कि दस्तावेज़ पृष्ठ से बारकोड कैसे निकाले जाएँ:

```csharp
// Parser class का एक instance बनाएं
using (Parser parser = new Parser(filePath))
{
    // दूसरे दस्तावेज़ पृष्ठ से बारकोड निकालें।
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(1);

    // बारकोड पर इटररेट करें
    foreach(PageBarcodeArea barcode in barcodes)
    {
        // पृष्ठ सूचकांक प्रिंट करें
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // बारकोड मान प्रिंट करें
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### संबंधित देखें

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(BarcodeOptions) {#getbarcodes_1}

कस्टमाइज़ेशन विकल्पों का उपयोग करके दस्तावेज़ से बारकोड निकालता है।

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(BarcodeOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| options | BarcodeOptions | बारकोड निष्कर्षण के विकल्प। |

### रिटर्न वैल्यू

[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) ऑब्जेक्ट्स का संग्रह; `null` यदि बारकोड निष्कर्षण समर्थित नहीं है।

### Examples

निम्न उदाहरण दिखाता है कि ऊपरी-दाएँ कोने से बारकोड कैसे निकाले जाएँ।

```csharp
// Parser class का एक instance बनाएं
using (Parser parser = new Parser(filePath))
{
    // बारकोड निष्कर्षण के लिए उपयोग किए जाने वाले विकल्प बनाएं
    BarcodeOptions options = new BarcodeOptions(new Rectangle(new Point(590, 80), new Size(150, 150)));
    // ऊपरी-दाएँ कोने से बारकोड निकालें।
    IEnumerable<PageBarcodeArea> barcodes = parser.GetBarcodes(options);

    // बारकोड पर इटररेट करें
    foreach (PageBarcodeArea barcode in barcodes)
    {
        // पृष्ठ सूचकांक प्रिंट करें
        Console.WriteLine("Page: " + barcode.Page.Index.ToString());
        // बारकोड मान प्रिंट करें
        Console.WriteLine("Value: " + barcode.Value);
    }
}
```

### संबंधित देखें

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [BarcodeOptions](../../../groupdocs.parser.options/barcodeoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetBarcodes(int, BarcodeOptions) {#getbarcodes_4}

कस्टमाइज़ेशन विकल्पों का उपयोग करके दस्तावेज़ पृष्ठ से बारकोड निकालता है।

```csharp
public IEnumerable<PageBarcodeArea> GetBarcodes(int pageIndex, BarcodeOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageIndex | Int32 | शून्य-आधारित पेज इंडेक्स। |
| options | BarcodeOptions | बारकोड निष्कर्षण के विकल्प। |

### रिटर्न वैल्यू

[`PageBarcodeArea`](../../../groupdocs.parser.data/pagebarcodearea) ऑब्जेक्ट्स का संग्रह; `null` यदि बारकोड निष्कर्षण समर्थित नहीं है।

### संबंधित देखें

* class [PageBarcodeArea](../../../groupdocs.parser.data/pagebarcodearea)
* class [BarcodeOptions](../../../groupdocs.parser.options/barcodeoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
