---
title: "GetTables"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "दस्तावेज़ से तालिकाएं निकालता है।"
type: docs
weight: 170
url: /hi/net/groupdocs.parser/parser/gettables/
---

## GetTables(PageTableAreaOptions) {#gettables_1}

दस्तावेज़ से तालिकाएं निकालता है।

```csharp
public IEnumerable<PageTableArea> GetTables(PageTableAreaOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| options | PageTableAreaOptions | टेबल निष्कर्षण के विकल्प। |

### रिटर्न वैल्यू

एक संग्रह [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) ऑब्जेक्ट्स का; यदि टेबल निष्कर्षण समर्थित नहीं है तो `null`।

### Examples

निम्नलिखित उदाहरण दिखाता है कि पूरे दस्तावेज़ से टेबल कैसे निकाली जाएँ:

```csharp
// Parser class का एक instance बनाएं
using (Parser parser = new Parser(filePath))
{
    // जाँचें कि दस्तावेज़ टेबल निष्कर्षण का समर्थन करता है या नहीं
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // टेबल का लेआउट बनाएं
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // टेबल निष्कर्षण के विकल्प बनाएं
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // दस्तावेज़ से टेबल निकालें
    IEnumerable<PageTableArea> tables = parser.GetTables(options);
    // तालिकाओं पर इटररेट करें
    foreach (PageTableArea t in tables)
    {
        // पंक्तियों पर इटररेट करें
        for (int row = 0; row < t.RowCount; row++)
        {
            // स्तंभों पर इटररेट करें
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // टेबल सेल प्राप्त करें
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // टेबल सेल का पाठ प्रिंट करें
                    Console.Write(cell.Text);
                    Console.Write(" | ");
                }
            }
            Console.WriteLine();
        }
        Console.WriteLine();
    }
}
```

### संबंधित देखें

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables(int, PageTableAreaOptions) {#gettables_3}

दस्तावेज़ पृष्ठ से तालिकाएँ निकालता है।

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex, PageTableAreaOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageIndex | Int32 | शून्य-आधारित पेज इंडेक्स। |
| options | PageTableAreaOptions | टेबल निष्कर्षण के विकल्प। |

### रिटर्न वैल्यू

एक संग्रह [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) ऑब्जेक्ट्स का; यदि टेबल निष्कर्षण समर्थित नहीं है तो `null`।

### Examples

निम्नलिखित उदाहरण दिखाता है कि दस्तावेज़ पृष्ठ से टेबल कैसे निकाली जाएँ:

```csharp
// Parser class का एक instance बनाएं
using (Parser parser = new Parser(filePath))
{
    // जाँचें कि दस्तावेज़ टेबल निष्कर्षण का समर्थन करता है या नहीं
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // टेबल का लेआउट बनाएं
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // टेबल निष्कर्षण के विकल्प बनाएं
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // दस्तावेज़ की जानकारी प्राप्त करें
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // जाँचें कि दस्तावेज़ में पृष्ठ हैं या नहीं
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("The document has no pages.");
        return;
    }
    // पृष्ठों पर इटररेट करें
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // पृष्ठ संख्या प्रिंट करें 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // दस्तावेज़ पृष्ठ से टेबल निकालें
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex, options);
        // तालिकाओं पर इटररेट करें
        foreach (PageTableArea t in tables)
        {
            // पंक्तियों पर इटररेट करें
            for (int row = 0; row < t.RowCount; row++)
            {
                // स्तंभों पर इटररेट करें
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // टेबल सेल प्राप्त करें
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // टेबल सेल का पाठ प्रिंट करें
                        Console.Write(cell.Text);
                        Console.Write(" | ");
                    }
                }
                Console.WriteLine();
            }
            Console.WriteLine();
        }
    }
}
```

### संबंधित देखें

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables() {#gettables}

दस्तावेज़ से तालिकाएं निकालता है।

```csharp
public IEnumerable<PageTableArea> GetTables()
```

### रिटर्न वैल्यू

एक संग्रह [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) ऑब्जेक्ट्स का; यदि टेबल निष्कर्षण समर्थित नहीं है तो `null`।

### Examples

निम्नलिखित उदाहरण दिखाता है कि पूरे दस्तावेज़ से टेबल कैसे निकाली जाएँ:

```csharp
// Parser class का एक instance बनाएं
using (Parser parser = new Parser(filePath))
{
    // जाँचें कि दस्तावेज़ टेबल निष्कर्षण का समर्थन करता है या नहीं
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // दस्तावेज़ से टेबल निकालें
    IEnumerable<PageTableArea> tables = parser.GetTables();
    // तालिकाओं पर इटररेट करें
    foreach (PageTableArea t in tables)
    {
        // पंक्तियों पर इटररेट करें
        for (int row = 0; row < t.RowCount; row++)
        {
            // स्तंभों पर इटररेट करें
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // टेबल सेल प्राप्त करें
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // टेबल सेल का पाठ प्रिंट करें
                    Console.Write(cell.Text);
                    Console.Write(" | ");
                }
            }
            Console.WriteLine();
        }
        Console.WriteLine();
    }
}
```

### संबंधित देखें

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## GetTables(int) {#gettables_2}

दस्तावेज़ पृष्ठ से तालिकाएँ निकालता है।

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageIndex | Int32 | शून्य-आधारित पेज इंडेक्स। |

### रिटर्न वैल्यू

एक संग्रह [`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) ऑब्जेक्ट्स का; यदि टेबल निष्कर्षण समर्थित नहीं है तो `null`।

### Examples

निम्नलिखित उदाहरण दिखाता है कि दस्तावेज़ पृष्ठ से टेबल कैसे निकाली जाएँ:

```csharp
// Parser class का एक instance बनाएं
using (Parser parser = new Parser(filePath))
{
    // जाँचें कि दस्तावेज़ टेबल निष्कर्षण का समर्थन करता है या नहीं
    if (!parser.Features.Tables)
    {
        Console.WriteLine("The document does not support tables extraction.");
        return;
    }
    // दस्तावेज़ की जानकारी प्राप्त करें
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // जाँचें कि दस्तावेज़ में पृष्ठ हैं या नहीं
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("The document has no pages.");
        return;
    }
    // पृष्ठों पर इटररेट करें
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // पृष्ठ संख्या प्रिंट करें 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // दस्तावेज़ पृष्ठ से टेबल निकालें
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex);
        // तालिकाओं पर इटररेट करें
        foreach (PageTableArea t in tables)
        {
            // पंक्तियों पर इटररेट करें
            for (int row = 0; row < t.RowCount; row++)
            {
                // स्तंभों पर इटररेट करें
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // टेबल सेल प्राप्त करें
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // टेबल सेल का पाठ प्रिंट करें
                        Console.Write(cell.Text);
                        Console.Write(" | ");
                    }
                }
                Console.WriteLine();
            }
            Console.WriteLine();
        }
    }
}
```

### संबंधित देखें

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
