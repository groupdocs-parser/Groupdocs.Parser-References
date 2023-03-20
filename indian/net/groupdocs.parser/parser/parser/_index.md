---
title: Parser
second_title: GroupDocs.Parser .NET API संदर्भ के लिए
description: क एक नय उदहरण प्ररंभ करत हैParsergroupdocs.parser/parser वर्ग एक डेटबेस से डेट नकलने के लए
type: docs
weight: 10
url: /hi/net/groupdocs.parser/parser/parser/
---
## Parser(DbConnection) {#constructor_2}

का एक नया उदाहरण प्रारंभ करता है[`Parser`](../../parser) वर्ग एक डेटाबेस से डेटा निकालने के लिए।

```csharp
public Parser(DbConnection connection)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| connection | DbConnection | डेटाबेस कनेक्शन। |

### टिप्पणियों

**और अधिक जानें:**

* [डेटाबेस से डेटा निकालें](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### उदाहरण

निम्न उदाहरण दिखाता है कि स्क्लाइट डेटाबेस से डेटा कैसे निकाला जाए:

```csharp
// DbConnection ऑब्जेक्ट बनाएं
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// डेटाबेस से टेबल निकालने के लिए पार्सर क्लास का एक उदाहरण बनाएं
using (Parser parser = new Parser(connection))
{
    // जांचें कि टेक्स्ट निष्कर्षण समर्थित है या नहीं
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // जांचें कि क्या toc निष्कर्षण समर्थित है
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // तालिकाओं की एक सूची प्राप्त करें
    IEnumerable<TocItem> toc = parser.GetToc();
    // तालिकाओं पर पुनरावृति करें
    foreach (TocItem i in toc)
    {
        // टेबल का नाम प्रिंट करें
        Console.WriteLine(i.Text);
        // तालिका की सामग्री को टेक्स्ट के रूप में निकालें
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### यह सभी देखें

* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

का एक नया उदाहरण प्रारंभ करता है[`Parser`](../../parser) वर्ग एक डेटाबेस से डेटा निकालने के लिए।

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| connection | DbConnection | डेटाबेस कनेक्शन। |
| parserSettings | ParserSettings | डेटा निष्कर्षण को अनुकूलित करने के लिए उपयोग की जाने वाली पार्सर सेटिंग्स। |

### टिप्पणियों

**और अधिक जानें:**

* [डेटाबेस से डेटा निकालें](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [लॉगिंग](https://docs.groupdocs.com/display/parsernet/Logging)

### उदाहरण

निम्न उदाहरण दिखाता है कि स्क्लाइट डेटाबेस से डेटा कैसे निकाला जाए:

```csharp
// DbConnection ऑब्जेक्ट बनाएं
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// डेटाबेस से टेबल निकालने के लिए पार्सर क्लास का एक उदाहरण बनाएं
using (Parser parser = new Parser(connection))
{
    // जांचें कि टेक्स्ट निष्कर्षण समर्थित है या नहीं
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // जांचें कि क्या toc निष्कर्षण समर्थित है
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // तालिकाओं की एक सूची प्राप्त करें
    IEnumerable<TocItem> toc = parser.GetToc();
    // तालिकाओं पर पुनरावृति करें
    foreach (TocItem i in toc)
    {
        // टेबल का नाम प्रिंट करें
        Console.WriteLine(i.Text);
        // तालिका की सामग्री को टेक्स्ट के रूप में निकालें
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### यह सभी देखें

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

का एक नया उदाहरण प्रारंभ करता है[`Parser`](../../parser) वर्ग एक दूरस्थ ईमेल सर्वर से डेटा निकालने के लिए।

```csharp
public Parser(EmailConnection connection)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| connection | EmailConnection | ईमेल कनेक्शन। |

### टिप्पणियों

**और अधिक जानें:**

* [POP, IMAP या Exchange Web Services प्रोटोकॉल के माध्यम से दूरस्थ सर्वर से ईमेल निकालें](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### उदाहरण

निम्न उदाहरण दिखाता है कि एक्सचेंज सर्वर से ईमेल कैसे निकालें:

```csharp
// एक्सचेंज वेब सर्विसेज प्रोटोकॉल के लिए कनेक्शन ऑब्जेक्ट बनाएं 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// दूरस्थ सर्वर से ईमेल निकालने के लिए पार्सर क्लास का एक उदाहरण बनाएं
using (Parser parser = new Parser(connection))
{
    // जांचें कि क्या कंटेनर निष्कर्षण समर्थित है
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// सर्वर से ईमेल संदेश निकालें
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // अनुलग्नकों पर पुनरावृति
    foreach (ContainerItem item in emails)
    {
        // ईमेल संदेश के लिए पार्सर वर्ग का एक उदाहरण बनाएँ
        using (Parser emailParser = item.OpenParser())
        {
            // ईमेल टेक्स्ट निकालें
            using (TextReader reader = emailParser.GetText())
            {
                // ईमेल टेक्स्ट प्रिंट करें
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### यह सभी देखें

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

का एक नया उदाहरण प्रारंभ करता है[`Parser`](../../parser) वर्ग एक दूरस्थ ईमेल सर्वर से डेटा निकालने के लिए।

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| connection | EmailConnection | ईमेल कनेक्शन। |
| parserSettings | ParserSettings | डेटा निष्कर्षण को अनुकूलित करने के लिए उपयोग की जाने वाली पार्सर सेटिंग्स। |

### टिप्पणियों

**और अधिक जानें:**

* [POP, IMAP या Exchange Web Services प्रोटोकॉल के माध्यम से दूरस्थ सर्वर से ईमेल निकालें](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [लॉगिंग](https://docs.groupdocs.com/display/parsernet/Logging)

### उदाहरण

निम्न उदाहरण दिखाता है कि एक्सचेंज सर्वर से ईमेल कैसे निकालें:

```csharp
// एक्सचेंज वेब सर्विसेज प्रोटोकॉल के लिए कनेक्शन ऑब्जेक्ट बनाएं 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// दूरस्थ सर्वर से ईमेल निकालने के लिए पार्सर क्लास का एक उदाहरण बनाएं
using (Parser parser = new Parser(connection))
{
    // जांचें कि क्या कंटेनर निष्कर्षण समर्थित है
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// सर्वर से ईमेल संदेश निकालें
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // अनुलग्नकों पर पुनरावृति
    foreach (ContainerItem item in emails)
    {
        // ईमेल संदेश के लिए पार्सर वर्ग का एक उदाहरण बनाएँ
        using (Parser emailParser = item.OpenParser())
        {
            // ईमेल टेक्स्ट निकालें
            using (TextReader reader = emailParser.GetText())
            {
                // ईमेल टेक्स्ट प्रिंट करें
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### यह सभी देखें

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_8}

का एक नया उदाहरण प्रारंभ करता है[`Parser`](../../parser) वर्ग.

```csharp
public Parser(string filePath)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | String | फ़ाइल का पथ। |

### टिप्पणियों

**और अधिक जानें:**

* [स्थानीय डिस्क से दस्तावेज़ लोड करें](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### उदाहरण

निम्न उदाहरण दिखाता है कि स्थानीय डिस्क से दस्तावेज़ को कैसे लोड किया जाए:

```csharp
// फाइलपाथ के साथ पार्सर क्लास का एक उदाहरण बनाएं
using (Parser parser = new Parser(filePath))
{
    // पाठक में एक पाठ निकालें
    using (TextReader reader = parser.GetText())
    {
        // दस्तावेज़ से एक पाठ प्रिंट करें
        // यदि पाठ निष्कर्षण समर्थित नहीं है, तो एक पाठक शून्य है
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### यह सभी देखें

* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_9}

का एक नया उदाहरण प्रारंभ करता है[`Parser`](../../parser) के साथ वर्ग[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) .

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | String | फ़ाइल का पथ। |
| loadOptions | LoadOptions | फ़ाइल खोलने के विकल्प। |

### टिप्पणियों

**और अधिक जानें:**

* [विशिष्ट फ़ाइल स्वरूपों को लोड करना](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [पासवर्ड से सुरक्षित दस्तावेज़ लोड हो रहे हैं](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [स्थानीय डिस्क से दस्तावेज़ लोड करें](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### उदाहरण

दस्तावेज़ पासवर्ड LoadOptions वर्ग द्वारा पारित किया गया है:

```csharp
try
{
    // पासवर्ड के साथ पार्सर क्लास का एक उदाहरण बनाएं:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // जांचें कि टेक्स्ट निष्कर्षण समर्थित है या नहीं
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // दस्तावेज़ टेक्स्ट प्रिंट करें
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // पासवर्ड गलत या खाली होने पर संदेश प्रिंट करें
    Console.WriteLine("Invalid password");
}
```

### यह सभी देखें

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

---

## Parser(string, ParserSettings) {#constructor_11}

का एक नया उदाहरण प्रारंभ करता है[`Parser`](../../parser) के साथ वर्ग[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(string filePath, ParserSettings parserSettings)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | String | फ़ाइल का पथ। |
| parserSettings | ParserSettings | डेटा निष्कर्षण को अनुकूलित करने के लिए उपयोग की जाने वाली पार्सर सेटिंग्स। |

### यह सभी देखें

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_10}

का एक नया उदाहरण प्रारंभ करता है[`Parser`](../../parser) के साथ वर्ग[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) और[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | String | फ़ाइल का पथ। |
| loadOptions | LoadOptions | फ़ाइल खोलने के विकल्प। |
| parserSettings | ParserSettings | डेटा निष्कर्षण को अनुकूलित करने के लिए उपयोग की जाने वाली पार्सर सेटिंग्स। |

### टिप्पणियों

**और अधिक जानें:**

* [विशिष्ट फ़ाइल स्वरूपों को लोड करना](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [पासवर्ड से सुरक्षित दस्तावेज़ लोड हो रहे हैं](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [लॉगिंग](https://docs.groupdocs.com/display/parsernet/Logging)
* [स्थानीय डिस्क से दस्तावेज़ लोड करें](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### उदाहरण

निम्न उदाहरण दिखाता है कि सूचना कैसे प्राप्त की जाए[`ILogger`](../../../groupdocs.parser.options/ilogger) इंटरफेस:

```csharp
// कोशिश
{
    // लकड़हारे वर्ग का एक उदाहरण बनाएँ
    Logger logger = new Logger();
    // पार्सर सेटिंग्स के साथ पार्सर क्लास का एक उदाहरण बनाएं
    using (Parser parser = new Parser(filePath, null, new ParserSettings(logger)))
    {
        // जांचें कि टेक्स्ट निष्कर्षण समर्थित है या नहीं
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // दस्तावेज़ टेक्स्ट प्रिंट करें
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // अपवाद पर ध्यान न दें
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // प्रिंट त्रुटि संदेश
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // प्रिंट घटना संदेश
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // प्रिंट चेतावनी संदेश
        Console.WriteLine("Warning: " + message);
    }
}
```

### यह सभी देखें

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

का एक नया उदाहरण प्रारंभ करता है[`Parser`](../../parser) वर्ग.

```csharp
public Parser(Stream document)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| document | Stream | स्रोत इनपुट स्ट्रीम। |

### टिप्पणियों

**और अधिक जानें:**

* [स्ट्रीम से दस्तावेज़ लोड करें](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### उदाहरण

निम्न उदाहरण दिखाता है कि दस्तावेज़ को स्ट्रीम से कैसे लोड किया जाए:

```csharp
// स्ट्रीम के साथ पार्सर क्लास का एक उदाहरण बनाएं
using (Parser parser = new Parser(stream))
{
    // पाठक में एक पाठ निकालें
    using (TextReader reader = parser.GetText())
    {
        // दस्तावेज़ से एक पाठ प्रिंट करें
        // यदि पाठ निष्कर्षण समर्थित नहीं है, तो एक पाठक शून्य है
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### यह सभी देखें

* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

का एक नया उदाहरण प्रारंभ करता है[`Parser`](../../parser) के साथ वर्ग[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) .

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| document | Stream | स्रोत इनपुट स्ट्रीम। |
| loadOptions | LoadOptions | फ़ाइल खोलने के विकल्प। |

### टिप्पणियों

**और अधिक जानें:**

* [विशिष्ट फ़ाइल स्वरूपों को लोड करना](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [पासवर्ड से सुरक्षित दस्तावेज़ लोड हो रहे हैं](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [स्ट्रीम से दस्तावेज़ लोड करें](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### उदाहरण

कुछ मामलों में इसे परिभाषित करना आवश्यक है[`FileFormat`](../../../groupdocs.parser.options/fileformat). दोनों विशेष मामलों (डेटाबेस, ईमेल सर्वर) और सामग्री द्वारा फ़ाइल प्रकारों का पता लगाने के लिए:

दस्तावेज़ पासवर्ड द्वारा पारित किया गया है[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) कक्षा:

```csharp
// मार्कडाउन दस्तावेज़ के लिए पार्सर वर्ग का एक उदाहरण बनाएँ
using (Parser parser = new Parser(stream, new LoadOptions(FileFormat.Markup)))
{
    // जांचें कि टेक्स्ट निष्कर्षण समर्थित है या नहीं
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    using (TextReader reader = parser.GetText())
    {
        // दस्तावेज़ टेक्स्ट प्रिंट करें
        // मार्कडाउन का पता चला है; विशेष प्रतीकों के बिना पाठ मुद्रित किया जाता है
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

```csharp
try
{
    // पासवर्ड के साथ पार्सर क्लास का एक उदाहरण बनाएं:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // जांचें कि टेक्स्ट निष्कर्षण समर्थित है या नहीं
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // दस्तावेज़ टेक्स्ट प्रिंट करें
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // पासवर्ड गलत या खाली होने पर संदेश प्रिंट करें
    Console.WriteLine("Invalid password");
}
```

### यह सभी देखें

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

---

## Parser(Stream, ParserSettings) {#constructor_7}

का एक नया उदाहरण प्रारंभ करता है[`Parser`](../../parser) के साथ वर्ग[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(Stream document, ParserSettings parserSettings)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| document | Stream | स्रोत इनपुट स्ट्रीम। |
| parserSettings | ParserSettings | डेटा निष्कर्षण को अनुकूलित करने के लिए उपयोग की जाने वाली पार्सर सेटिंग्स। |

### यह सभी देखें

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

का एक नया उदाहरण प्रारंभ करता है[`Parser`](../../parser) के साथ वर्ग[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) और[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| document | Stream | स्रोत इनपुट स्ट्रीम। |
| loadOptions | LoadOptions | फ़ाइल खोलने के विकल्प। |
| parserSettings | ParserSettings | डेटा निष्कर्षण को अनुकूलित करने के लिए उपयोग की जाने वाली पार्सर सेटिंग्स। |

### टिप्पणियों

**और अधिक जानें:**

* [विशिष्ट फ़ाइल स्वरूपों को लोड करना](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [पासवर्ड से सुरक्षित दस्तावेज़ लोड हो रहे हैं](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [स्ट्रीम से दस्तावेज़ लोड करें](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [लॉगिंग](https://docs.groupdocs.com/display/parsernet/Logging)

### उदाहरण

निम्न उदाहरण दिखाता है कि सूचना कैसे प्राप्त की जाए[`ILogger`](../../../groupdocs.parser.options/ilogger) इंटरफेस:

```csharp
// कोशिश
{
    // लकड़हारे वर्ग का एक उदाहरण बनाएँ
    Logger logger = new Logger();
    // पार्सर सेटिंग्स के साथ पार्सर क्लास का एक उदाहरण बनाएं
    using (Parser parser = new Parser(stream, null, new ParserSettings(logger)))
    {
        // जांचें कि टेक्स्ट निष्कर्षण समर्थित है या नहीं
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // दस्तावेज़ टेक्स्ट प्रिंट करें
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // अपवाद पर ध्यान न दें
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // प्रिंट त्रुटि संदेश
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // प्रिंट घटना संदेश
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // प्रिंट चेतावनी संदेश
        Console.WriteLine("Warning: " + message);
    }
}
```

### यह सभी देखें

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* नाम स्थान [GroupDocs.Parser](../../parser)
* सभा [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
