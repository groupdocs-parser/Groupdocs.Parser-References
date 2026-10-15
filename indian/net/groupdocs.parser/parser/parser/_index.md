---
title: "पार्सर"
second_title: "GroupDocs.Parser के लिए .NET API संदर्भ"
description: "एक URI से डेटा निकालने के लिए Parsergroupdocs.parser/parser क्लास की नई इंस्टेंस को प्रारंभ करता है।"
type: docs
weight: 10
url: /hi/net/groupdocs.parser/parser/parser/
---

## Parser(Uri) {#constructor_12}

एक URI से डेटा निकालने के लिए [`Parser`](../../parser) क्लास की नई इंस्टेंस को प्रारंभ करता है।

```csharp
public Parser(Uri uri)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| uri | Uri | वह Uri जिस पर अनुरोध भेजा जाता है। |

### संबंधित देखें

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, LoadOptions) {#constructor_13}

एक URI से डेटा निकालने के लिए *loadOptions* के साथ [`Parser`](../../parser) क्लास की नई इंस्टेंस को प्रारंभ करता है।

```csharp
public Parser(Uri uri, LoadOptions loadOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| uri | Uri | वह Uri जिस पर अनुरोध भेजा जाता है। |
| loadOptions | LoadOptions | फ़ाइल खोलने के विकल्प। |

### संबंधित देखें

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, ParserSettings) {#constructor_15}

एक URI से डेटा निकालने के लिए *parserSettings* के साथ [`Parser`](../../parser) क्लास की नई इंस्टेंस को प्रारंभ करता है।

```csharp
public Parser(Uri uri, ParserSettings parserSettings)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| uri | Uri | वह Uri जिस पर अनुरोध भेजा जाता है। |
| parserSettings | ParserSettings | डेटा निष्कर्षण को अनुकूलित करने के लिए उपयोग किए जाने वाले पार्सर सेटिंग्स। |

### संबंधित देखें

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Uri, LoadOptions, ParserSettings) {#constructor_14}

एक URI से डेटा निकालने के लिए *loadOptions* और *parserSettings* के साथ [`Parser`](../../parser) क्लास की नई इंस्टेंस को प्रारंभ करता है।

```csharp
public Parser(Uri uri, LoadOptions loadOptions, ParserSettings parserSettings)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| uri | Uri | वह Uri जिस पर अनुरोध भेजा जाता है। |
| loadOptions | LoadOptions | फ़ाइल खोलने के विकल्प। |
| parserSettings | ParserSettings | डेटा निष्कर्षण को अनुकूलित करने के लिए उपयोग किए जाने वाले पार्सर सेटिंग्स। |

### संबंधित देखें

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(DbConnection) {#constructor_2}

डेटाबेस से डेटा निकालने के लिए [`Parser`](../../parser) क्लास की नई इंस्टेंस को प्रारंभ करता है।

```csharp
public Parser(DbConnection connection)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| कनेक्शन | DbConnection | डेटाबेस कनेक्शन। |

### टिप्पणियाँ

**Learn more:**

* [Extract data from databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### Examples

निम्न उदाहरण दिखाता है कि कैसे Sqlite डेटाबेस से डेटा निकाला जाए:

```csharp
// DbConnection ऑब्जेक्ट बनाएं
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// डेटाबेस से तालिकाएँ निकालने के लिए Parser क्लास की एक इंस्टेंस बनाएं
using (Parser parser = new Parser(connection))
{
    // जाँचें कि क्या पाठ निष्कर्षण समर्थित है
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // जाँचें कि toc निष्कर्षण समर्थित है या नहीं
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // तालिकाओं की सूची प्राप्त करें
    IEnumerable<TocItem> toc = parser.GetToc();
    // तालिकाओं पर इटररेट करें
    foreach (TocItem i in toc)
    {
        // तालिका का नाम प्रिंट करें
        Console.WriteLine(i.Text);
        // एक तालिका की सामग्री को टेक्स्ट के रूप में निकालें
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### संबंधित देखें

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

डेटाबेस से डेटा निकालने के लिए [`Parser`](../../parser) क्लास की नई इंस्टेंस को प्रारंभ करता है।

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| कनेक्शन | DbConnection | डेटाबेस कनेक्शन। |
| parserSettings | ParserSettings | डेटा निष्कर्षण को अनुकूलित करने के लिए उपयोग किए जाने वाले पार्सर सेटिंग्स। |

### टिप्पणियाँ

**Learn more:**

* [Extract data from databases](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Examples

निम्न उदाहरण दिखाता है कि कैसे Sqlite डेटाबेस से डेटा निकाला जाए:

```csharp
// DbConnection ऑब्जेक्ट बनाएं
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// डेटाबेस से तालिकाएँ निकालने के लिए Parser क्लास की एक इंस्टेंस बनाएं
using (Parser parser = new Parser(connection))
{
    // जाँचें कि क्या पाठ निष्कर्षण समर्थित है
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // जाँचें कि toc निष्कर्षण समर्थित है या नहीं
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // तालिकाओं की सूची प्राप्त करें
    IEnumerable<TocItem> toc = parser.GetToc();
    // तालिकाओं पर इटररेट करें
    foreach (TocItem i in toc)
    {
        // तालिका का नाम प्रिंट करें
        Console.WriteLine(i.Text);
        // एक तालिका की सामग्री को टेक्स्ट के रूप में निकालें
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### संबंधित देखें

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

रिमोट ईमेल सर्वर से डेटा निकालने के लिए [`Parser`](../../parser) क्लास की नई इंस्टेंस को प्रारंभ करता है।

```csharp
public Parser(EmailConnection connection)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| कनेक्शन | EmailConnection | ईमेल कनेक्शन। |

### टिप्पणियाँ

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### Examples

निम्न उदाहरण दिखाता है कि कैसे Exchange Server से ईमेल निकाले जाएँ:

```csharp
// Exchange Web Services प्रोटोकॉल के लिए कनेक्शन ऑब्जेक्ट बनाएं 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// रिमोट सर्वर से ईमेल निकालने के लिए Parser क्लास की एक इंस्टेंस बनाएं
using (Parser parser = new Parser(connection))
{
    // जाँचें कि कंटेनर निष्कर्षण समर्थित है या नहीं
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// सर्वर से ईमेल संदेश निकालें
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // संलग्नकों पर पुनरावृत्ति करें
    foreach (ContainerItem item in emails)
    {
        // ईमेल संदेश के लिए Parser क्लास का एक उदाहरण बनाएं
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

### संबंधित देखें

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

रिमोट ईमेल सर्वर से डेटा निकालने के लिए [`Parser`](../../parser) क्लास की नई इंस्टेंस को प्रारंभ करता है।

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| कनेक्शन | EmailConnection | ईमेल कनेक्शन। |
| parserSettings | ParserSettings | डेटा निष्कर्षण को अनुकूलित करने के लिए उपयोग किए जाने वाले पार्सर सेटिंग्स। |

### टिप्पणियाँ

**Learn more:**

* [Extract emails from remote server via POP, IMAP or Exchange Web Services protocols](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Examples

निम्न उदाहरण दिखाता है कि कैसे Exchange Server से ईमेल निकाले जाएँ:

```csharp
// Exchange Web Services प्रोटोकॉल के लिए कनेक्शन ऑब्जेक्ट बनाएं 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// रिमोट सर्वर से ईमेल निकालने के लिए Parser क्लास की एक इंस्टेंस बनाएं
using (Parser parser = new Parser(connection))
{
    // जाँचें कि कंटेनर निष्कर्षण समर्थित है या नहीं
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// सर्वर से ईमेल संदेश निकालें
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // संलग्नकों पर पुनरावृत्ति करें
    foreach (ContainerItem item in emails)
    {
        // ईमेल संदेश के लिए Parser क्लास का एक उदाहरण बनाएं
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

### संबंधित देखें

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_8}

[`Parser`](../../parser) क्लास का एक नया उदाहरण प्रारंभ करता है।

```csharp
public Parser(string filePath)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | स्ट्रिंग | फ़ाइल का पथ। |

### टिप्पणियाँ

**Learn more:**

* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Examples

निम्नलिखित उदाहरण दिखाता है कि स्थानीय डिस्क से दस्तावेज़ कैसे लोड करें:

```csharp
// filePath के साथ Parser क्लास का एक उदाहरण बनाएं
using (Parser parser = new Parser(filePath))
{
    // पाठ को रीडर में निकालें
    using (TextReader reader = parser.GetText())
    {
        // दस्तावेज़ से पाठ प्रिंट करें
        // यदि पाठ निष्कर्षण समर्थित नहीं है, तो रीडर `null` होगा
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### संबंधित देखें

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_9}

[`Parser`](../../parser) क्लास का एक नया उदाहरण [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) के साथ प्रारंभ करता है।

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | स्ट्रिंग | फ़ाइल का पथ। |
| loadOptions | LoadOptions | फ़ाइल खोलने के विकल्प। |

### टिप्पणियाँ

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Examples

दस्तावेज़ पासवर्ड LoadOptions क्लास द्वारा पास किया जाता है:

```csharp
try
{
    // पासवर्ड के साथ Parser क्लास का एक उदाहरण बनाएं:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // जाँचें कि क्या पाठ निष्कर्षण समर्थित है
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
    // यदि पासवर्ड गलत या खाली है तो संदेश प्रिंट करें
    Console.WriteLine("Invalid password");
}
```

### संबंधित देखें

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, ParserSettings) {#constructor_11}

[`Parser`](../../parser) क्लास का एक नया उदाहरण [`ParserSettings`](../../../groupdocs.parser.options/parsersettings) के साथ प्रारंभ करता है।

```csharp
public Parser(string filePath, ParserSettings parserSettings)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | स्ट्रिंग | फ़ाइल का पथ। |
| parserSettings | ParserSettings | डेटा निष्कर्षण को अनुकूलित करने के लिए उपयोग किए जाने वाले पार्सर सेटिंग्स। |

### संबंधित देखें

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_10}

[`Parser`](../../parser) क्लास का एक नया उदाहरण [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) और [`ParserSettings`](../../../groupdocs.parser.options/parsersettings) के साथ प्रारंभ करता है।

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| filePath | स्ट्रिंग | फ़ाइल का पथ। |
| loadOptions | LoadOptions | फ़ाइल खोलने के विकल्प। |
| parserSettings | ParserSettings | डेटा निष्कर्षण को अनुकूलित करने के लिए उपयोग किए जाने वाले पार्सर सेटिंग्स। |

### टिप्पणियाँ

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)
* [Load document from local disk](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Examples

निम्नलिखित उदाहरण दिखाता है कि [`ILogger`](../../../groupdocs.parser.options/ilogger) इंटरफ़ेस के माध्यम से जानकारी कैसे प्राप्त करें:

```csharp
// try
{
    // Logger क्लास का एक उदाहरण बनाएं
    Logger logger = new Logger();
    // parser settings के साथ Parser क्लास का एक उदाहरण बनाएं
    using (Parser parser = new Parser(filePath, null, new ParserSettings(logger)))
    {
        // जाँचें कि क्या पाठ निष्कर्षण समर्थित है
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
    ; // Ignore the exception
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // त्रुटि संदेश प्रिंट करें
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // इवेंट संदेश प्रिंट करें
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // चेतावनी संदेश प्रिंट करें
        Console.WriteLine("Warning: " + message);
    }
}
```

### संबंधित देखें

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

[`Parser`](../../parser) क्लास का एक नया उदाहरण प्रारंभ करता है।

```csharp
public Parser(Stream document)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| दस्तावेज़ | Stream | स्रोत इनपुट स्ट्रीम। |

### टिप्पणियाँ

**Learn more:**

* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Examples

निम्नलिखित उदाहरण दिखाता है कि स्ट्रीम से दस्तावेज़ कैसे लोड करें:

```csharp
// स्ट्रीम के साथ Parser क्लास का एक उदाहरण बनाएं
using (Parser parser = new Parser(stream))
{
    // पाठ को रीडर में निकालें
    using (TextReader reader = parser.GetText())
    {
        // दस्तावेज़ से पाठ प्रिंट करें
        // यदि पाठ निष्कर्षण समर्थित नहीं है, तो रीडर `null` होगा
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### संबंधित देखें

* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

[`Parser`](../../parser) क्लास का एक नया उदाहरण [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) के साथ प्रारंभ करता है।

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| दस्तावेज़ | Stream | स्रोत इनपुट स्ट्रीम। |
| loadOptions | LoadOptions | फ़ाइल खोलने के विकल्प। |

### टिप्पणियाँ

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Examples

कुछ मामलों में [`FileFormat`](../../../groupdocs.parser.options/fileformat) को परिभाषित करना आवश्यक होता है। विशेष मामलों (डेटाबेस, ईमेल सर्वर) और सामग्री के आधार पर फ़ाइल प्रकार का पता लगाने के लिए दोनों।

```csharp
// Markdown दस्तावेज़ के लिए Parser क्लास का एक उदाहरण बनाएं
using (Parser parser = new Parser(stream, new LoadOptions(FileFormat.Markup)))
{
    // जाँचें कि क्या पाठ निष्कर्षण समर्थित है
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    using (TextReader reader = parser.GetText())
    {
        // दस्तावेज़ टेक्स्ट प्रिंट करें
        // Markdown का पता लगाया गया; विशेष प्रतीकों के बिना पाठ प्रदर्शित किया जाता है
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

दस्तावेज़ पासवर्ड को [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) क्लास द्वारा पास किया जाता है:

```csharp
try
{
    // पासवर्ड के साथ Parser क्लास का एक उदाहरण बनाएं:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // जाँचें कि क्या पाठ निष्कर्षण समर्थित है
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
    // यदि पासवर्ड गलत या खाली है तो संदेश प्रिंट करें
    Console.WriteLine("Invalid password");
}
```

### संबंधित देखें

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, ParserSettings) {#constructor_7}

[`Parser`](../../parser) क्लास का एक नया उदाहरण [`ParserSettings`](../../../groupdocs.parser.options/parsersettings) के साथ प्रारंभ करता है।

```csharp
public Parser(Stream document, ParserSettings parserSettings)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| दस्तावेज़ | Stream | स्रोत इनपुट स्ट्रीम। |
| parserSettings | ParserSettings | डेटा निष्कर्षण को अनुकूलित करने के लिए उपयोग किए जाने वाले पार्सर सेटिंग्स। |

### संबंधित देखें

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

[`Parser`](../../parser) क्लास का एक नया उदाहरण [`LoadOptions`](../../../groupdocs.parser.options/loadoptions) और [`ParserSettings`](../../../groupdocs.parser.options/parsersettings) के साथ प्रारंभ करता है।

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| दस्तावेज़ | Stream | स्रोत इनपुट स्ट्रीम। |
| loadOptions | LoadOptions | फ़ाइल खोलने के विकल्प। |
| parserSettings | ParserSettings | डेटा निष्कर्षण को अनुकूलित करने के लिए उपयोग किए जाने वाले पार्सर सेटिंग्स। |

### टिप्पणियाँ

**Learn more:**

* [Loading specific file formats](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Loading password-protected documents](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Load document from stream](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [Logging](https://docs.groupdocs.com/display/parsernet/Logging)

### Examples

निम्नलिखित उदाहरण दिखाता है कि [`ILogger`](../../../groupdocs.parser.options/ilogger) इंटरफ़ेस के माध्यम से जानकारी कैसे प्राप्त करें:

```csharp
// try
{
    // Logger क्लास का एक उदाहरण बनाएं
    Logger logger = new Logger();
    // parser settings के साथ Parser क्लास का एक उदाहरण बनाएं
    using (Parser parser = new Parser(stream, null, new ParserSettings(logger)))
    {
        // जाँचें कि क्या पाठ निष्कर्षण समर्थित है
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
    ; // Ignore the exception
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // त्रुटि संदेश प्रिंट करें
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // इवेंट संदेश प्रिंट करें
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // चेतावनी संदेश प्रिंट करें
        Console.WriteLine("Warning: " + message);
    }
}
```

### संबंधित देखें

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* namespace [GroupDocs.Parser](../../../groupdocs.parser)
* assembly [GroupDocs.Parser](../../../)

<!-- संपादित न करें: xmldocmd द्वारा GroupDocs.Parser.dll के लिए उत्पन्न किया गया -->
