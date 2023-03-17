---
title: GetTables
second_title: GroupDocs.Parser .NET API संदर्भ के लिए
description: दस्तवेज़ से तलकएँ नकलत है
type: docs
weight: 140
url: /hi/net/groupdocs.parser/parser/gettables/
---
## GetTables(PageTableAreaOptions) {#gettables}

दस्तावेज़ से तालिकाएँ निकालता है।

```csharp
public IEnumerable<PageTableArea> GetTables(PageTableAreaOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| options | PageTableAreaOptions | तालिका निष्कर्षण के लिए विकल्प। |

### प्रतिलाभ की मात्रा

का संग्रह[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) ऑब्जेक्ट्स; `व्यर्थ` यदि तालिका निष्कर्षण समर्थित नहीं है.

### उदाहरण

निम्न उदाहरण दिखाता है कि पूरे दस्तावेज़ से तालिकाओं को कैसे निकाला जाए:

```csharp
// पार्सर वर्ग का एक उदाहरण बनाएँ
using (Parser parser = new Parser(filePath))
{
    // जांचें कि क्या दस्तावेज़ तालिका निष्कर्षण का समर्थन करता है
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // टेबल का लेआउट बनाएं
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // तालिका निष्कर्षण के लिए विकल्प बनाएँ
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // दस्तावेज़ से टेबल निकालें
    IEnumerable<PageTableArea> tables = parser.GetTables(options);
    // तालिकाओं पर पुनरावृति करें
    foreach (PageTableArea t in tables)
    {
        // पंक्तियों पर पुनरावृति करें
        for (int row = 0; row < t.RowCount; row++)
        {
            // स्तंभों पर पुनरावृति करें
            for (int column = 0; column < t.ColumnCount; column++)
            {
                // टेबल सेल प्राप्त करें
                PageTableAreaCell cell = t[row, column];
                if (cell != null)
                {
                    // टेबल सेल टेक्स्ट प्रिंट करें
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

### यह सभी देखें

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

---

## GetTables(int, PageTableAreaOptions) {#gettables_1}

दस्तावेज़ पृष्ठ से टेबल निकालता है.

```csharp
public IEnumerable<PageTableArea> GetTables(int pageIndex, PageTableAreaOptions options)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pageIndex | Int32 | शून्य-आधारित पृष्ठ अनुक्रमणिका। |
| options | PageTableAreaOptions | तालिका निष्कर्षण के लिए विकल्प। |

### प्रतिलाभ की मात्रा

का संग्रह[`PageTableArea`](../../../groupdocs.parser.data/pagetablearea) ऑब्जेक्ट्स; `व्यर्थ` यदि तालिका निष्कर्षण समर्थित नहीं है.

### उदाहरण

निम्न उदाहरण दिखाता है कि दस्तावेज़ पृष्ठ से तालिकाओं को कैसे निकाला जाए:

```csharp
// पार्सर वर्ग का एक उदाहरण बनाएँ
using (Parser parser = new Parser(filePath))
{
    // जांचें कि क्या दस्तावेज़ तालिका निष्कर्षण का समर्थन करता है
    if (!parser.Features.Tables)
    {
        Console.WriteLine("Document isn't supports tables extraction.");
        return;
    }
    // टेबल का लेआउट बनाएं
    TemplateTableLayout layout = new TemplateTableLayout(
        new double[] { 50, 95, 275, 415, 485, 545 },
        new double[] { 325, 340, 365, 395 });
    // तालिका निष्कर्षण के लिए विकल्प बनाएँ
    PageTableAreaOptions options = new PageTableAreaOptions(layout);
    // दस्तावेज़ की जानकारी प्राप्त करें
    IDocumentInfo documentInfo = parser.GetDocumentInfo();
    // जांचें कि क्या दस्तावेज़ में पृष्ठ हैं
    if (documentInfo.PageCount == 0)
    {
        Console.WriteLine("Document hasn't pages.");
        return;
    }
    // पृष्ठों पर पुनरावृति
    for (int pageIndex = 0; pageIndex < documentInfo.PageCount; pageIndex++)
    {
        // पेज नंबर प्रिंट करें 
        Console.WriteLine(string.Format("Page {0}/{1}", pageIndex + 1, documentInfo.PageCount));
        // दस्तावेज़ पृष्ठ से तालिकाएँ निकालें
        IEnumerable<PageTableArea> tables = parser.GetTables(pageIndex, options);
        // तालिकाओं पर पुनरावृति करें
        foreach (PageTableArea t in tables)
        {
            // पंक्तियों पर पुनरावृति करें
            for (int row = 0; row < t.RowCount; row++)
            {
                // स्तंभों पर पुनरावृति करें
                for (int column = 0; column < t.ColumnCount; column++)
                {
                    // टेबल सेल प्राप्त करें
                    PageTableAreaCell cell = t[row, column];
                    if (cell != null)
                    {
                        // टेबल सेल टेक्स्ट प्रिंट करें
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

### यह सभी देखें

* class [PageTableArea](../../../groupdocs.parser.data/pagetablearea)
* class [PageTableAreaOptions](../../../groupdocs.parser.options/pagetableareaoptions)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
